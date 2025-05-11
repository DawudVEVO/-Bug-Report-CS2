# -Bug-Report-CS2
 Bug Report: CS2 FPS Drops to 60 While Spectating, Fixes When UI Is Open
System Information
Game: Counter-Strike 2

Platform: Windows 11 (or 10, update if needed)

GPU: NVIDIA RTX 2080 SUPER

CPU: Intel Core i9-10900K

RAM: 32 GB DDR4

Monitor Refresh Rate: (e.g., 144Hz / 240Hz)

V-Sync: Disabled

Launch Options: -novid -high -nojoy +fps_max 300


Issue Description
While spectating in CS2 (after dying), my FPS consistently drops from ~280 FPS to exactly 60 FPS, despite my CPU and GPU usage dropping to 10–20%. This only happens in CS2 — not in any other Source or non-Source games.

The issue goes away instantly under two conditions:

If I press Escape to open the settings menu.

If I press Tab to open the scoreboard.

Once I open either menu, the FPS jumps back up to ~280 and stays there until the next round starts or I die again.

This strongly suggests the game engine is downclocking or throttling rendering while spectating and not properly resuming full performance when it should.


Troubleshooting Done
V-Sync off in game and control panel

Power plan set to High Performance

NVIDIA settings: Prefer maximum performance

Disabled overlays (Discord, Steam, GeForce)

Mat_queue_mode tested (0, 1, 2)

Clean config and verified game files

Confirmed issue is not present in other games

Expected Behavior
When spectating, FPS should remain consistent with when playing — no performance throttling unless intentionally enabled by the player.


Actual Behavior
FPS drops to 60 only while spectating; returns to normal when interacting with UI.




