# Tailwind equivalents

Use arbitrary values; never Tailwind's stock `shadow-*`, `border*`, `rounded-none`/`rounded-sm`, `bg-white`/`bg-black`, or `bg-gradient-*`.

| Role | Classes |
|---|---|
| Page | `bg-[#e0e5ec] text-[#333333]` |
| Card | `bg-[#e0e5ec] rounded-2xl p-6 md:p-8 shadow-[4px_4px_8px_#b8bcc2,-4px_-4px_8px_#ffffff] md:shadow-[8px_8px_16px_#b8bcc2,-8px_-8px_16px_#ffffff]` |
| Button | `bg-[#e0e5ec] rounded-xl min-h-11 px-5 font-semibold text-[#3d434c] shadow-[6px_6px_12px_#b8bcc2,-6px_-6px_12px_#ffffff] hover:shadow-[3px_3px_6px_#b8bcc2,-3px_-3px_6px_#ffffff] active:shadow-[inset_4px_4px_8px_#b8bcc2,inset_-4px_-4px_8px_#ffffff] transition-shadow duration-300 ease-in-out focus-visible:outline-2 focus-visible:outline-offset-3 focus-visible:outline-[#6d5dfc]` |
| Primary button | the button classes with `bg-[#6d5dfc] text-white active:shadow-[inset_4px_4px_8px_#5246c9,inset_-4px_-4px_8px_#8a7dff]` |
| Input | `bg-[#e0e5ec] rounded-xl px-4 min-h-11 shadow-[inset_6px_6px_12px_#b8bcc2,inset_-6px_-6px_12px_#ffffff] focus:outline-none focus:shadow-[inset_2px_2px_4px_#b8bcc2,inset_-2px_-2px_4px_#ffffff,0_0_0_2px_#6d5dfc] transition-shadow duration-300 ease-in-out` |
| Well | `bg-[#e0e5ec] rounded-2xl p-4 shadow-[inset_4px_4px_8px_#b8bcc2,inset_-4px_-4px_8px_#ffffff]` |
| Heading / body / secondary | `text-[#2b2f36] font-semibold` / `text-[#333333]` / `text-[#545b66]` |

Don't use `hover:scale-*`, `translate-*`, or `duration-200` on controls (always `duration-300 ease-in-out`). Add `motion-reduce:transition-none` to transitions.
