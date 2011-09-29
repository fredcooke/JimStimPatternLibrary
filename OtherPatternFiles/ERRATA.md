### Errata For This File

Note the file that is included here is included as-is from jbperf.com and may
contain errors. In this file you will have the date that the file was pulled
from jbperf.com and any known errors with it.

Date: Sept 22nd through Oct 3rd 2011, and before.

Errors:

1. Mitsi 4/1 CAS - This pattern is completely wrong with various edges not falling where they should, making using it for development of a high quality engine controller impossible. I personally know someone who had major trouble with the 3.1.1, and probably later, MS2Extra code developed using this pattern. MS users, beware!!
2. Mitsi DSM/Miata 4/2 CAS - This pattern has the edges aligned correctly and is pretty close to the truth. My numbers vary from this by a little, however it is, as the yanks say, good enough for government work. The same friend swapped to the MS2Extra implementatin of this and has had no further trouble.
3. GM LT1 Optispark CAS 360 and 8 - While it is possible that more than one variant exists, it seems very unlikely. The pattern included here has all of the unique and narrow slots off by exactly 2. Given the sensitive nature of these CAS units I would NOT recommend using the MS3 implementation of this. In order for it to function it must be doing something called sloppy sync. Though statistically unlikely, it is possible for noise to come in on both signals in appropriate ratios and render the decoder significantly wrong for a single cycle, enough to schedule some ignition events early and do harm. More advanced implementations contain checks for this and would never sync on such a wrong pattern. If the decoder was written to sync on this, and also syncs on the real thing, then it is far far FAR too relaxed in what it accepts. Additionally, even with the pattern corrected it is not stable above 4600 and completely wrong above 6100. Beware!!

Please also note that, by and large, MegaSquirt firmware variants were developed against this file and variants of it. As such if you're using a MegaSquirt decoder for one of the patterns mentioned here, be VERY wary.

