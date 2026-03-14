Tired of jittery FPS? **Advanced FPS Limiter** replaces Minecraft’s loose FPS limiter with rock-solid, precise frame
pacing for a butter-smooth experience.

---

### What this mod does

This mod greatly improves minecraft's native FPS limiter. <br>
This can help with:

* more stable frame rate
* lower power consumption (especially useful for laptop users)
* smoother and more consistent gameplay

Limiting FPS is especially useful when your system produces far more frames than your monitor can display, which
otherwise causes unnecessary GPU workload.

---

### When this mod is useful

This mod is particularly useful if you:

* want to cap your FPS to an exact value (for example 60, 90 or 120)
* want stable frame pacing
* want to reduce unnecessary GPU usage

---

### Technical

**Advanced FPS Limiter** replaces the internal `limitDisplayFPS` logic with a high-precision hybrid waiting loop. By
utilizing `glfwWaitEventsTimeout` and `LockSupport.parkNanos`, it hits the frame target with near-perfect accuracy
without burning your CPU.