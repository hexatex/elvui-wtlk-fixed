# elvui wtlk (3.3.5) fixed

This is my own version of the elvui addon where I am doing my own bug fixes and enhancements.

## Fixed Issues

### Nameplate Style Filtering Debuff Bug
A "timeLeft" variable was being set to nil in pdateElement_AuraIcons which causes the "aura filter check" in StyleFilterAuraCheck to fail. That made it so that the filter would almost never match, or would match one second then not match the next, or vice versa. I removed the line setting time left to nil and it works!
