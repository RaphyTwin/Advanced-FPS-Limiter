Tired of jittery FPS? **Advanced FPS Limiter** replaces Minecraft’s loose FPS limiter with rock-solid, precise frame
pacing for a butter-smooth experience.

#

### The Problem: Vanilla's "Suggestion"

Most players don't realize that Minecraft’s built-in FPS limiter is more of a suggestion than a rule. Even when locked
at 60 FPS, the game often delivers frames at irregular intervals, leading to micro-stuttering and uneven frame times.

<br>

### The Solution: Precision Control

**Advanced FPS Limiter** reworks the internal timing engine to ensure that your frames are delivered exactly when they
should be. No more spikes, no more jitter—just a nearly perfectly flat frame-time graph.

---

### Technical

**Advanced FPS Limiter** replaces the internal `limitDisplayFPS` logic with a high-precision hybrid waiting loop. By
utilizing `glfwWaitEventsTimeout` and `LockSupport.parkNanos`, it hits the frame target with near-perfect accuracy
without burning your CPU.