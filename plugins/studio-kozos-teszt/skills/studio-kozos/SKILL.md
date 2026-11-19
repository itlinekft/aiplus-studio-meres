---
name: studio-kozos
description: Use when the person says "közös plugin teszt" or asks which Studio sites are connected. Measurement skill.
---

# Közös plugin teszt

1. Write first, on its own line: `KOZOS-JEL v0.1.1`.
2. Find every tool whose name ends in `studio_allapot`. Each one belongs to one connected Studio.
3. Call each of them once. From each answer take the site's name and host.
4. List the sites as `- <name> · <host> · <the tool name prefix>`.
5. If there is more than one, ask the person with AskUserQuestion which site to work on (one option per site).
   If there is exactly one, say that one is used. If there is none, write:
   „Nincs bekötött Studio. Kösd be a Studio connectort, aztán kérd újra.” and stop.
6. After the choice, call the chosen site's `studio_allapot` again and write: `KIVALASZTVA: <host>`.
