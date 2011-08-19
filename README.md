= TRIM patcher =

Based on Grant Pannell [information](http://digitaldj.net/2011/07/21/trim-enabler-for-lion/) about how to patch
Lion properly to enable TRIM support on non-Apple branded
SSDs, here's a script that ought to make it harder to shoot
yourself in the foot.

== Usage ==

To use this, simply start up a terminal and run the script.

== Available arguments ==

    --apply     applies the patch, after making sure we know the
                file we're applying to, backing it up only if it's
                the original one, and subsequently checking if the
                patch applied correctly.
    --revert    reverts the patch, after making sure we're working
                on the patched file, and afterward checks for correct
                reversion.
    --restore   restores from the previously made backup.
    --status    shows current situation, including status of the file
                and whether a backup is available.

In any case of success, the kext cache gets cleared.
