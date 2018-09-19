# TV-off-box

The fancy new smart tv that I got for christmas just won't stay off. Not to mention that the US and foreign intelligence agencies are longing to use smart tvs and other IOT devices that are otherwise sitting around connected to the internet.

I have no evidence that I am being targeted, but I know that my tv is a more powerful computer than the CRTs or yore and shouldn't be trusted in standby by itself. My TV off box watches for the on signal from the remote or button and handles connecting and disconnecting the tv.

## Details

1. The tv takes some time to boot up, and that time differs depending on whether or not the ethernet is connected. For maximum compatibility, there needs to be a delay between when the TV-on-box recieves the on signal and when it actually turns the tv on based on the longest amount of time it would take the machine to boot. 

2. The TV **doesn't** remember it's state. It always boots to standby. The off box uses an IR led to transmitt the on signal to the tv after the tv boots to standby.

3. Both the on button and the IR transiever must line up in the code flow so that both interfaces can be used. For example, I should be able to turn the tv on with the remote, and then turn it off with the button or vice versa.

