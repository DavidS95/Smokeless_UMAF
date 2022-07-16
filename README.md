# Smokeless_UMAF 
# Bios Flasher Where We’re Going, We Don’t Need Bios Flasher?
What this can do
With this tool you can Access and modify AMD PBS/AMD CBS Menu and possibly AMD Overclocking without flashing, and by just booting from a USB drive

Disclaimer
I'm not responsible for any damage resulting from the use of this Tool;

USE AT YOUR OWN RISK

Using this tool you agree also to this rule Think twice before committing any change

Changing setting could lead to brick, so handle with care, and be sure to have a method to recovery your device if things go wrong.

Know Problem (Read This)
Dell User have reported than the normal bios will not load anymore after using this :

Fix Thank to (BIT_GAM3R and the Gaming Laptop Mod Discord Comunity): https://discord.com/invite/FDgUR5cpCg

Boot the Tool, access the BootManager, and delete the Misc Option, they should not be there, are created by a bug, if you tryed access the BootManager Before... Proper Fix will be pushed when ready

Might not work on some Bios like the Thinkpad one (No solution Yet)

Dangerous Setting
Know setting that will make your device brick

P0State Vid
How this work
AMD PBS/AMD CBS and possibly AMD Overclocking (Aod_Setup) export their HII database regardless of the manufacturer, so if we can load these we can access these menus without problem.

This package includes two main component a Loader and the UI component, the latter one are build from a standard edk2 Package. On boot from usb the Loader will unregister the existing bios FormBrowser and will load this custom one, proving the new interface for this boot.

The interface is a bit oldish, but get the work done...

The only drawback of this method is that you need to boot from USB to accessed these menus.

How to use it
Extract in a FAT32 USB, and boot from it, it will load the custom bios UI, Now if you enter Device Manager, AMD PBS/CBS will be there, you can modify what you want, and when done, just hit esc until it ask you to save.

On AMI Bios, in addition to AMD PBS and CBS will be shown also "Setup", this is the regular bios, the edit here might not be saved (AMD PBS/CBS, Aod Setup)
