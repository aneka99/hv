Protecting hard drives against data loss
Protecting hard drives is best done using a [hard disk backup software](https://backupchain.com/i/disk-cloning) or [file backup solution](https://backupchain.com/en/backup-software/), but one must remember that repeated copies impose stress on these devices. However, mechanical protection is also important.

Parking the heads

To protect the surfaces of the disks from being hit by the read/write heads (the so-called head crash), the heads move to the landing zone, where they are fixed, even before the rotational speed has noticeably reduced when the hard disk is switched off. When the supply voltage is suddenly removed, the drive is switched as a generator and the energy thus obtained is used to generate a swivel pulse for the head arm. This parking increases the shock resistance of the disks for transport or conversion. The parking position can be outside the disks or inside the disks. In this case, the read/write head touches down on a predefined area of the disk that does not contain any data. The surface of this area is specially pre-treated to prevent the head from sticking, thus enabling the hard disk to be restarted later. The fixation is done, for example, by a magnet that holds the read head in place. 
In older hard disks, the read/write heads were moved out of the disk stack in almost all models. Later (1990s, 2000s), a parking position inside was increasingly preferred. In 2008, both variants occur. For notebook disks, the parking position outside the disk stack provides additional protection against damage to the surfaces of the disks during transport (vibration) of the hard disk. 
With older hard disks, the heads had to be explicitly parked by command from the operating system before being switched off - stepper motors required many coordinated pulses for parking, which were very difficult or impossible to generate after the supply voltage was removed. The heads of modern hard disks can also be explicitly parked, since the described automatic parking mechanism can lead to increased wear after the supply voltage is removed. Today, the park command is sent automatically by the device driver when the system is shut down. 
In modern laptops, an acceleration sensor ensures that the hard disk finger is parked even during a possible free fall in order to limit the damage when a computer falls. 

Hard disk case

The housing of a hard disk is very massive. Usually it is a casting made of an aluminum alloy and covered with a stainless steel sheet cover. If a hard disk is opened in normal, uncleaned air, even the smallest dust or smoke particles, fingerprints, etc. can cause irreparable damage to the disk surfaces and the read/write heads. 
The enclosure is dust-tight, but is usually not sealed airtight in the case of air-filled drives. Air can enter or leave through a small opening fitted with a filter in the event of air pressure fluctuations (such as occur with temperature changes or changes in atmospheric air pressure) to compensate for the pressure differences. This opening - see adjacent figure - must not be closed. Since the air pressure in the housing decreases with increasing altitude above sea level, but a minimum pressure is required for operation, these hard disks may only be operated up to a certain maximum sea level. This is usually noted in the associated data sheet. The air is required to prevent direct contact between the read/write head and the data carrier surface (head crash); see also section The read/write head unit above. In newer drives, an elastic diaphragm is used instead of the filter, which allows the system to adapt to changing pressure conditions by bulging in one direction or the other. 
Some hard drive models are filled with helium and, unlike air-filled drives, are hermetically sealed. Helium has a lower density and higher thermal conductivity compared to air. Helium's lower density results in fewer disruptive flow effects, leading to reduced forces acting on the motor. Vibrations caused by the positioning of the carrier arms are also reduced. As a result, the distances between the individual disks can be reduced and more of them can be integrated with the same overall height, leading to a higher storage density for these disk drives


Installation

Until around the 1990s, hard disks required a defined installation position and usually only horizontal operation (but not "overhead") or vertical position ("on edge") was permitted. This is no longer required or specified for today's drives; they can be operated in any position. All hard disks are sensitive to vibration during operation, as this can disturb the positioning of the heads. If a hard disk is elastically mounted, this point must be given special consideration. 
Until around the 1990s, a defined installation position was required for hard disks and usually only horizontal operation (but not "overhead") or vertical position ("on the edge") was permitted. This is no longer required or specified for today's drives; they can be operated in any position. All hard disks are sensitive to vibration during operation, as this can disturb the positioning of the heads. If a hard disk is elastically mounted, this point must be given special consideration. 


Storing and reading bits

The disk with the magnetic layer in which the information is stored rotates past the read/write heads (see above). During reading, changes in the magnetization of the surface cause a voltage pulse in the read head due to electromagnetic induction. Until the beginning of the 21st century, longitudinal recording was used almost exclusively; only then was perpendicular recording introduced, which allows much higher write densities but causes smaller signals during reading, making it more difficult to control. For writing, the same head is used to write the information into the magnetic layer. For reading, a magnetic head should be designed differently than for writing, for example in terms of the width of the magnetic gap; if it is used for both, compromises must be made that again limit performance. There are newer approaches to this by using special geometries and coil windings to make these compromises more efficient. 
Thus, a read pulse occurs only when the magnetization changes (mathematically: the read head "sees", so to speak, only the derivative of the magnetization according to the spatial coordinate). These pulses form a serial data stream, which is evaluated by the reading electronics as with a serial interface. If, for example, data are present that happen to have only the logical level "0" over long distances, no change occurs for as long as this is the case, i.e. there is no signal at the read head. The read electronics can then get out of sync and read incorrect values. To remedy this, various procedures are used that insert additional reverse-poled bits into the data stream to avoid an excessively long stretch of uniform magnetization. Examples of these procedures are MFM and RLL, the general technique is explained under line code. 
During the write operation, a current of different polarity is fed into the magnetic coil of the write head (opposite polarity, but same strength), depending on the logic level of the bit. The current causes a magnetic field, the field is bundled and guided by the magnetic core of the head. In the gap of the write head, the magnetic field lines then enter the surface of the hard disk, magnetizing it in the desired direction. 
Storing and reading byte-organized data.


Today's magnetic hard disks organize their data - in contrast to random access memories (which arrange them in bytes or in small groups of 2 to 8 bytes) - in data blocks (such as 512, 2048 or 4096 bytes), which is why this method is called block-based addressing. Only whole data blocks or sectors can be read and written on the part of the interface. (With earlier SCSI hard disks, the drive electronics enabled byte-by-byte access). 
Blocks are read by specifying the linear sector number. The hard disk "knows" where this block is located and reads or writes it on demand. 


When writing blocks: 

- they are first provided with error correction information (forward error correction),

- they are subjected to modulation: In former times GCR, MFM, RLL were common, nowadays PRML and recently EPRML have replaced them, then

- the read/write head carrier is moved to the vicinity of the track to be written to,

- the read/write head, which is assigned to the information-carrying surface, reads the track signal and carries out the fine positioning. On the one hand, this involves finding the correct track and, on the other, hitting this track exactly in the center.

- If the read/write head is stable on the track and the correct sector is located under the read/write head, the block modulation is written.

- In the event of a suspected incorrect position, the write process must be aborted immediately so that no neighboring tracks are destroyed (sometimes irreparably).

 
During reading, these steps are carried out in reverse: 

- Move the read/write head carrier close to the track that is to be read.
- 
- the read/write head, which is assigned to the information-carrying surface, reads the track signal and performs the fine positioning.
- 
- Now the track is read as long (or a little longer) until the desired sector has been found successfully.

