# Troubleshooting

This guide covers common problems with Presence Manager and how to solve them.

## The presence does not appear on Discord

1. Make sure **Discord Desktop is running** — Presence Manager only connects while Discord is open.
2. Open the application and check the home page: it should show **Discord: Connected**.
3. Make sure you clicked **Apply Presence** (or enabled "Apply when Discord opens" in the settings).
4. Check that **Presence is active** on the home page.

## "Informe o Application ID" when applying

- The **Application ID** field is empty or invalid. Open the **Presence** page, paste the Application ID of your application from the [Discord Developer Portal](https://discord.com/developers/applications), and click **Save Configuration** before applying.

## Connection to Discord fails

- Discord Desktop may be closed. Open Discord and wait — the application reconnects automatically.
- Your internet connection may be offline.
- The Application ID may be invalid or the application may have been deleted in the Developer Portal.
- Use **Test Connection** on the home page to check the state.

## The presence disappears when Discord closes

- This is expected. Presence Manager monitors Discord and reconnects + re-applies your presence automatically when Discord opens again (if automatic reconnection is enabled in the settings).

## Settings are not saved

- The application writes to `%AppData%\PresenceManager`. Make sure that folder is writable (antivirus software can sometimes block writes).
- If a file becomes unreadable, the application logs the error and uses the default settings; a `.corrupt` copy of the file may be created.

## The application does not start with Windows

- Enable **Start with Windows** in the **Settings** page. The application registers itself in the Windows startup entries (per-user, no administrator privileges required).
- Keep the executable in a fixed location: if you move the application after enabling this option, the startup entry will point to the old path.

## The elapsed timer does not start where I expected

- On the **Presence** page, the "Start of the counter" option controls this:
  - **When activating the presence** — the counter starts at 0 when you apply.
  - **Specific date and time** — the counter already shows the time elapsed since that date/time.
- A date in the future is adjusted automatically so the counter starts at 0.

## Images do not appear in the presence

- Image keys must match the names of the **Rich Presence Assets** registered in the [Discord Developer Portal](https://discord.com/developers/applications) (Rich Presence → Art Assets).
- The application does not upload images: it only references assets that already exist in your Discord application.

## Buttons do not appear

- Buttons with a URL only work with the `https://` or `http://` protocol. The Discord client ignores URLs that do not follow this rule.
- If a label exceeds the allowed length (32 characters), the field may be ignored by Discord.

## I need more details / the log

The application writes a log file to:

```
%AppData%\PresenceManager\presence-manager.log
```

Open the **Settings** page and use **Open folder** to access it. When reporting a problem, including the relevant part of this log helps a lot.

> **Important:** when sharing logs or reports, do not include tokens, passwords, private Application IDs or personal information.
