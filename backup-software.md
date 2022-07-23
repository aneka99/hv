Anti-virus programs are good to have; however, they only offer partial protection against data loss. The best solution against data loss is still having a [reliable backup software](https://backupchain.com/en/backupchain/). But what is the history of anti-virus tools and how did they become popular?

Most of the computer viruses written in the early and mid-1980s were limited to pure self-replication and often did not necessarily have a specific malicious function. It was not until the technique of virus programming became known to wider circles that malicious programs that specifically manipulated or destroyed data on infected computers began to appear. This created the need to worry about fighting these malicious programs with special anti-virus programs.

There are competing claims as to who is the inventor of the first antivirus program. The first program to combat the Creeper worm on ARPA-Net was developed back in 1971. Probably the first publicly documented removal of a computer virus with a tool was done by Bernd Fix in 1987. Fred Cohen, who had already made the subject of "computer viruses" public through his work in 1984, developed strategies for combating viruses from 1988 onwards, which were taken up and continued by later anti-virus programmers. 
Also in 1988, a mailing list called VIRUS-L was created in the BITNET/EARN computer network, which mainly discussed the emergence of new viruses as well as ways to combat them. Some participants of this list, such as John McAfee or Eugene Kaspersky, subsequently founded companies that developed and offered commercial anti-virus programs. Four years earlier, in 1984, Arcen Data (now Norman ASA) had already been founded, which also specialized in antivirus programs at the end of the 1980s, when the first computer viruses appeared in Norway. In 1987, the G DATA Software company introduced the world's first commercial antivirus program, developed specifically for the Atari ST.  Before Internet connectivity became common, viruses typically spread via floppy disks. Antivirus programs were sometimes used, but only irregularly updated to a current state. During this time, antivirus programs only checked executable programs and the boot sectors on floppy disks and hard drives. With the spread of the Internet, viruses began to infect new computers in this way, posing a more general threat.
Over time, it became increasingly important for antivirus programs to scan different file types (and not just executable programs) for hidden viruses. This was for a variety of reasons: 

- The use of macros in word processing programs such as Microsoft Word posed an additional virus risk. Virus programmers began embedding viruses as macros in documents. This meant that computers could be infected simply by running an embedded macro virus in a document.


Later email programs, particularly Microsoft Outlook Express and Outlook, were vulnerable to viruses embedded in email. This allowed a computer to be infected by opening and viewing an email.
As the number of existing viruses increased, it also became necessary to update antivirus programs frequently. But even under these circumstances, a new type of virus could spread widely within a short period of time before antivirus manufacturers could respond by updating them.

Real-time scanner

The real-time scanner, also called access scanner or resident scanner, is active in the background as a system service (Windows) or daemon (Unix) and scans all files, programs, memory and possibly HTTP as well as FTP traffic. To achieve this, so-called filter drivers are installed by the antivirus program, which provide the interface between the real-time scanner and the file system. If the real-time scanner finds something suspicious, it usually asks the user what to do next. This is to block access, delete the file, move it to quarantine or, if possible, attempt to repair it. In general, real-time protection can be divided into two strategies: 
1. scanning when opening files (read operation).
2. scanning when creating / modifying files (write operation)

It may be the case that a virulent file was saved before a virus signature was available for it. However, after a signature update, it is possible to detect it when it is opened. So in this case, scanning when the file is opened is superior to scanning when the file is written. In order to reduce the load of the real-time scanner, some file formats, compressed files (archives) or similar are often scanned only partially or not at all. 

Manual ScannerThe manual scanner also called file scanner, must be started by the user manually or scheduled (on-demand). If a scanner finds malicious software, a warning message appears and usually also a request for the desired action: cleaning, quarantine or deletion of the infected file(s). 


Online virus scanner

Online virus scanners are antivirus programs that load their program code and virus patterns over a network (online). Unlike permanently installed virus scanners, they operate only in on-demand mode. This means that the persistent protection provided by an on-access mode is not guaranteed. Online virus scanners are often also used as so-called second-opinion scanners, in order to obtain a "second opinion" on possible infestations in addition to the installed virus scanner. 
Furthermore, there are websites that make it possible to scan individual files with different virus scanners. For this type of scan, the user himself must actively upload the file, so it is a special form of on-demand scan. 





