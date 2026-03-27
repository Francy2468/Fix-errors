# Fix-errors
try to dump all files with entire output
+ try to do 100% unc and env
Sometimes it confuses a loadstring and assigns it as a local library when it should be a normal one. I just want it to detect if it's a library or not. If it is a library, assign it as local; if not, don't assign it as local library. 
Output not generated: [string "Obfuscated_Script"]:1: <name> expected near 'nil'
Add dump with code block example: .l ```print("hi")```
Output not generated: [string "Obfuscated_Script"]:455: unexpected symbol near ':'
Output not generated: [string "Obfuscated_Script"]:1: 'until' expected near 'end'
Try to dump thid aswell:
https://gitlab.com/rlbx-scripts/elysium-sab/-/raw/main/elysium-sab
if the bot detects @everyone or @here put that he dosent write that in the output or message because it could get spammed the bot need to skip @pings 
