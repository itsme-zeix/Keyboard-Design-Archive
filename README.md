# Table of Contents
- [PCB Designs](#pcb-designs)

  - [SingaKBD x Rubrehose x KLC Playground Rubrehaku](#singakbd-x-rubrehose-x-klc-playground-rubrehaku)
  - [SingaKBD Kohaku R2 Soldered & Hotswap](#singakbd-kohaku-r2-soldered--hotswap)
  - [Lain](#lain) 
  - [DN Alisea](#dn-alisea)
  - [DN Seven](#dn-seven)
  - [DN 925](#dn-925)
  - [DN Realforce Daughterboard](#dn-realforce-daughterboard)
  - [Typface Univers Soldered & Hotswap 70%](#typface-univers-soldered--hotswap-70)
  - [DN 997.3/765LT/SVJ TKLs](#dn-9973765ltsvj-tkls)
  - [qwertyqop QQ60 Hotswap PCB](#qwertyqop-qq60-hotswap-pcb)
  - [Trial PCB Art](#trial-pcb-art)
  - [DN Numpad](#dn-numpad)
  - [KAI Eden](#kai-eden)
  - [Hex Keyboards HEX.4B v2 Solder/Hotswap](#hex-keyboards-hex4b-v2-solderhotswap)
  - [DN FRLTKL (HITC/DNDD)](#dn-frltkl-hitcdndd)
  - [shostudios Burrito](#shostudios-burrito)
  - [shostudios Chums](#shostudios-chums)
  - [Banana Stand Works Vomit Comet](#banana-stand-works-vomit-comet)
  - [DN SBL](#dn-sbl)
- [zeta.keyboard projects](#zetakeyboard-projects)
  - [Hera R2](#hera-r2)
  - [Hera Alpha Edition (R1)](#hera-alpha-edition-r1)


# PCB Designs
Note that the list of projects below is non-exhaustive. There are projects still in the works and also others that I have probably forgotten about. Here are some interesting functional features of my designs:
- I typically avoid SOD diodes in favour of standard 0805 diodes which are less likely to shear off.
- I use larger sized throughhole pads and teardrops in hopes that the pads will adhere better and be less likely to lift when soldering.

For commissions or inquiries, please direct message me on Discord @zeix.
### SingaKBD x Rubrehose x KLC Playground Rubrehaku
To be added

### SingaKBD Kohaku R2 Soldered & Hotswap
To be added

### Lain
This project was a one off commission designed in collaboration with yz for Squashy Boy. You can check out his video [here](https://youtu.be/KJbTZ06ZaB4?si=rEDmcRYNUsHE81eT)!

This design features a TFT display implemented using the SPI protocol and QMK's Quantum Painter API. One of the (frankly unexpected) challenge faced was that using a high-bitrate GIF caused significant input delay or even missed inputs. This issue arose because QMK runs on a single thread, forcing it to divide processing time between sending GIF frames and doing matrix scanning for keyboard inputs.

We ended up making a compromise by having a 'boot-up' GIF played when the keyboard plugged in, which then transitions to a static image of the GIF's final frame. Using a static image resolved this issue as it didn't require constant data transfer to update frames.

For future iterations, I would probably use a separate microcontroller dedicated to the display.

<img src="https://github.com/itsme-zeix/Past-Keyboard-Work/assets/102467346/1776e69d-0b11-4421-b921-47999bfa80e9" alt="lain" width="500">

### DN Alisea
To be added

### DN Seven
To be added

### DN 925 
To be added

### DN Realforce Daughterboard
To be added

### Typface Univers Soldered & Hotswap 70%
![SCR-20240428-ldav](https://github.com/itsme-zeix/Past-Keyboard-Work/assets/102467346/97e010a5-a032-498d-82c1-b30fe7c6941e)
![SCR-20240428-lcsm](https://github.com/itsme-zeix/Past-Keyboard-Work/assets/102467346/0bcff966-2239-493d-bf1e-10045154a10f)
Images retrieved from [nearLucid's review](https://www.youtube.com/watch?v=-D23rrUj9Og)

### DN 997.3/765LT/SVJ TKLs
![SVJ_front](https://github.com/itsme-zeix/Past-Keyboard-Work/assets/102467346/61b85ef1-157b-482a-8c12-b3d466ad0a0b)
![SVJ_Back](https://github.com/itsme-zeix/Past-Keyboard-Work/assets/102467346/843396ba-9dc0-47c1-8e6b-63a8f90a4e2f)
<img src="https://github.com/itsme-zeix/Past-Keyboard-Work/assets/102467346/08c12ac6-ff4a-46e8-8e71-fa183e1e2af2" alt="765lt" width="500">

### qwertyqop QQ60 Hotswap
A versatile 60% hotswap PCB designed with H60 compatability. It can be purchased [here](https://qwertyqop.com/products/qq60) (assuming it's in stock).

This was my first project trialing TTC sockets due to their smaller footprint, particularly at edge cutouts where standard Kailh sockets tend to protrude. While the design isn't perfect—some cutout positions require trimming—cutouts at these position are rarely used (I think only Kei comes to mind?).

Additionally, it also supports an alternate JST port position to support the Unikorn R2.2.

![qq proto 2](https://github.com/itsme-zeix/Past-Keyboard-Work/assets/102467346/267357ec-522a-416e-a060-835b6453ae99)
![QQ60_production](https://github.com/itsme-zeix/Past-Keyboard-Work/assets/102467346/f8a0cab9-ece6-4c18-851a-11233342b915)

### Trial PCB Art
This project was  inspired by some PCBs I saw that used a mix of silkscreen, soldermask, exposed copper and exposed substrate to achieve multiple colours on a graphic. This project never actually got produced, but it was a cool proof of concept.

<img src="https://github.com/itsme-zeix/Past-Keyboard-Work/assets/102467346/fefdeb3a-c165-4ca8-86c4-2d317119f85e" alt="ExposedCopperTrial" width="600">

I also played around a little with rounded traces in this design too.

<img src="https://github.com/itsme-zeix/Past-Keyboard-Work/assets/102467346/ae5afc8e-262c-4982-ad5c-26a9d0da3b97" alt="RoundedTraces" width="600">


### DN Numpad
Peep the idb60 and the NEAT glass that I used for coffee!

<img src="https://github.com/itsme-zeix/Past-Keyboard-Work/assets/102467346/01ae3189-a3eb-4b33-9aac-797385bc1fb1" alt="RoundedTraces" width="600">

### KAI Eden ##
Unfortunately, I don't have pictures for this. It was a 60% PCB with holes for tadpole mount, nothing particularly different here. This is the [IC link](https://geekhack.org/index.php?topic=120074) if you want to check it out.

### Hex Keyboards HEX.4B v2 solder/hotswap
These are solder and hotswap prototypes I designed for the HEX.4B v2. Although this version never went into production, elements of its design and layout were later reused in later projects.

![4bv2 protos](https://github.com/itsme-zeix/Past-Keyboard-Work/assets/102467346/de2bc97e-06ed-45b8-959b-dfbfd315735b)

### DN FRLTKL (HITC/DNDD)
<img src="https://github.com/itsme-zeix/Past-Keyboard-Work/assets/102467346/47ee4f83-aca6-41eb-a9c5-722f802baa56" alt="hitc-proto" width="600">

<img src="https://github.com/itsme-zeix/Past-Keyboard-Work/assets/102467346/8b47955b-9f22-4d20-8ca0-d518863a3852" alt="factory-pink-dndd-image" width="600">

This was my first time trying pink soldermask. Really like how the colour turned out. (apologies for image quality, the photo was taken by the factory)

### shostudios Burrito
This was an interesting project. A full-size keyboard (minus the F-row) that required a significant number of pins. To reduce the number of microcontroller pins required by the matrix, I used a duplex matrix (it was my first time doing it here!).

![image (1)](https://user-images.githubusercontent.com/102467346/226098075-13269a90-e03b-4652-a3c9-43256e1b4de5.png)
<img src="https://user-images.githubusercontent.com/102467346/226098082-88393bac-b7e3-4517-8ff9-0756d7c693c3.jpg" alt="burrito-close-up" width="600">

### shostudios Chums
![20230216_181513](https://user-images.githubusercontent.com/102467346/226097872-8e12c6f2-3846-464f-adca-0bbcfec778c4.jpg)
![20230216_181501](https://user-images.githubusercontent.com/102467346/226097875-f5982999-ab76-4117-b3d4-9a3f668e2cf9.jpg)
![image (2)](https://user-images.githubusercontent.com/102467346/226097890-1ca7064c-05cf-4a5f-aa47-d45ab901af27.png)

### Banana Stand Works Vomit Comet
This was my first time trying out rounded traces.

![PXL_20230315_204825491](https://user-images.githubusercontent.com/102467346/226097712-35feb36d-294a-4b4b-9e3a-a9972b1ce75c.jpg)
![PXL_20230315_204857785](https://user-images.githubusercontent.com/102467346/226097716-d36a5a8d-e367-4727-b186-02887de0d4ed.jpg)
![image](https://user-images.githubusercontent.com/102467346/226097916-25c6da1c-e53f-4986-80da-34dfb8f68765.png)

### DN SBL
My first large scale project for a client!

#### Prototypes:
![20230310_144543](https://user-images.githubusercontent.com/102467346/226098255-d037797b-41fa-4ee3-9952-6a230c7f2b07.jpg)
![20230310_144535](https://user-images.githubusercontent.com/102467346/226098256-62e49426-3029-475b-9529-ca9199efaa72.jpg)

#### Production:
![20230525_201936](https://github.com/itsme-zeix/Past-Keyboard-Work/assets/102467346/92bfab6d-32a0-42cd-9968-c7f341eff673)
![20230525_201612](https://github.com/itsme-zeix/Past-Keyboard-Work/assets/102467346/9e4cf452-f570-4662-910a-9f3bea6ec4c8)


#### Hera PCB
Made for zeta.keyboards Hera. It was based off the existing open-sourced plain60. This was the first commercial project I worked on! Scroll down to read more about it.

# zeta.keyboard projects
## Hera R2 ##

A budget 60% keyboard focused on a flexy and bouncy typing experience. This was my first commercial venture, which I collaborated on with my friend Tarquin.

To achieve desired "bouncy" typing feel, Hera R2 features a half plate with a 1.2mm PCB that has a flex cut between rows 2 and 3. This design was inspired by (https://youtu.be/sqwuRAf8uas?si=ydKGngmbg8rbDVq6)[Velvet's OTD356mini] which also utilized a half plate with a similar PCB.

#### This was a re-run of the Hera Alpha Edition with some design changes:
  - Rounded back of aluminium case
  - Reduced distance between case floor and PCB
  - Switched from aluminium to FR4 plates to reduce pinging
  - Added a front lip
  - Decreased the size of the channel for the JST cable

#### Retailed for $320SGD for the base kit which includes:
  - Hera Case (available in Silver, Black or Lilac) with a sandblasted brass weight
  - 1.2mm PCB, daughterboard and JST cable
  - FR4 Half Plate
  - Carrying Case
  - 50A and 70A O Ring
  - Necessary screws

### Images 
**Image courtesy of Stack on Discord:**  
<img src="https://github.com/itsme-zeix/Past-Keyboard-Work/assets/102467346/281eda49-2ef7-4fd2-9ac7-f23a5d25cb97" alt="HeraImageByStack" width="600">

**Images courtesy of Kaitodesu (@mcdomnalds on Instagram):**
![DSC0868](https://github.com/itsme-zeix/Past-Keyboard-Work/assets/102467346/f7c7bd76-37f1-4bbc-bd47-e165705341db)
<img src="https://github.com/itsme-zeix/Past-Keyboard-Work/assets/102467346/eb53e3a7-9831-4d2e-bd81-2957f09f2f84" alt="HeraSideProfileShotByKaitodesu" width="600">

 **Images courtesy of Mecha Store:**  
![HeraColoursShotByMecha](https://user-images.githubusercontent.com/102467346/226122161-d891fc4b-1454-4044-9fed-ff7105e9bf54.jpg)

<img src="https://user-images.githubusercontent.com/102467346/226122168-acdee775-094e-4358-8542-173d8222c669.jpg" alt="HeraShotByMecha" width="600">

<img src="https://user-images.githubusercontent.com/102467346/226122181-1a6c1c8c-805a-4810-9afd-28c4ed8e3507.jpg" alt="HeraBackLogoShotByMecha" width="600">


<img src="https://user-images.githubusercontent.com/102467346/226122187-0f67638b-0713-4c6d-8038-93c3f938cbba.jpg" alt="HeraPlateShotByMecha" width="600">

![HeraCarryingCaseShotByMecha](https://user-images.githubusercontent.com/102467346/226122273-40f332e5-d56a-4661-8b26-270bdd3c6b7d.jpg)

 **Renders courtesy of aja:**
![7hera](https://user-images.githubusercontent.com/102467346/226098937-a8ba6841-630e-4630-8da5-fc7dfa8697c2.png)
![5hera](https://user-images.githubusercontent.com/102467346/226098945-d6500693-ed9f-4e41-8f8c-255a076d1d85.png)

**Some images from the R2 design phase**
![IMG-20210608-WA0009](https://user-images.githubusercontent.com/102467346/226123901-8b373491-9e36-44c2-aa0e-f13f3956132e.jpg)
![IMG-20210725-WA0016](https://user-images.githubusercontent.com/102467346/226123904-87159960-addf-4cea-ac69-5b14976e46c4.jpg)


## Hera Alpha Edition (R1) ##
This was designed off the open sourced Bakeneko (I think it was either v1 or v2?). We did a prototype FNF run to test out our design - manufactured using a sussy Taobao manufacturer Tarquin found. 

Unfortunately no images at the moment, maybe I'll add it in one day.

Here are it's features:
 - Black anodized case, brushed brass weight, aluminium half plate.
 - PCB was based off the open-sourced plain60, which I modified to add a flex cut between rows 2 and 3.
