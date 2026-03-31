# SDA Missing Title Issue Example

We're having a bit of trouble getting our SDA pages into WCAG 2.1 AA compliance. The issue is the lack of an h1 header where we expect one to be emitted. Below are instructions for reproducing the issue.

## Reproduction
1. `/path/to/sda/makesda -l us1850a.ddl -d us1850a.dat`
2. `/path/to/sda/xcodebk -b us1850a_codebook_commands.dat`
3. Observe that `Doc/nes.htm` has an empty h1 heading. We believe the study title should be there. The study title is specified as "United States 1850" in `us1850a.ddl` and `STUDYINF/studyinf`
