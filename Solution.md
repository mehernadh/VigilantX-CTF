# VNR VigilantX — OSINT CTF Solutions

**Note:** This write-up is being pushed to the same repository where the Git & Seek challenge was originally designed. However, the challenge can still be solved and the flag can be recovered as intended.

---

## Coordinates Over Lunch
**Image:** Coordinates Over Lunch.jpg
**Difficulty:** Easy 
**Flag Format:** `Fl4g-X{latitude,longitude}`  
**Flag:** `Fl4g-X{17.42, 78.41}`

### Challenge Description
A quick lunch break turned into a mystery. The photo was taken in a place famous for its cozy cafés and classic cars. Use your investigation skills to uncover the exact location.

### Solution
1. When we open the image we observe a food outlet. By carefully zooming in and inspecting the branding it becomes clear that the outlet shown is a Subway restaurant.
2. Reading the challenge description closely we notice the hint mentioning cozy cafés and classic cars. Since the challenge is set in Hyderabad this strongly points toward popular upscale localities such as Jubilee Hills or Banjara Hills.
3. Next we search for Subway outlets located in Jubilee Hills and Banjara Hills. By comparing Google Maps listings and reviewing available images one particular location stands out as a strong match.
4. Further investigation reveals that this Subway outlet in Jubilee Hills is located alongside Ariko Cafe. The surroundings and visual elements perfectly match the image provided in the challenge.
5. Finally we extract the geographical coordinates of Ariko Cafe using Google Maps. These coordinates represent the final flag for the challenge.

---

## Git & Seek
**Link:** [https://github.com/mehernadh/VigilantX-CTF.git](https://github.com/mehernadh/VigilantX-CTF.git) 
**Difficulty:** Easy  
**Flag Format:** `Fl4g-X{}`  
**Flag:** `Fl4g-X{tag_message_flag}`

### Challenge Description
Whenever CTF organizers create a challenge, they usually drop a GitHub repo and ask you to do some “random stuff.” Can you dig through it and find the hidden flag?

### Solution
1. On carefully reading the challenge description, it hints that CTF organizers often release challenges through a GitHub repository. This strongly suggests that a public repository exists for this challenge and needs to be discovered and explored.
2. We navigate to GitHub and search for repositories related to the challenge name `VigilantX`. During this search, we find a repository named `VigilantX-CTF` matching the challenge name.
3. After locating the repository, we begin exploring its contents to identify any hidden information or clues that may lead to the flag.
4. While browsing the repository, we observe that it contains three branches. However, none of these branches reveal anything useful. Further inspection shows the presence of a tag. Upon opening the tag, we discover the following encoded string `U3k0dC1Le2dudF96cmZmbnRyX3N5bnR9`
5. At first glance, the string resembles Base64 encoding. Decoding it using Base64 reveals the following output `Sy4t-K{gnt_zrffntr_synt}`
6. The decoded text appears to be obfuscated using a rotation cipher. Applying a common ROT13 transformation successfully reveals the final flag `Fl4g-X{tag_message_flag}`

---

## Beneath the Signal’s Hum
**Video:** Beneath the Signal’s Hum.mp4
**Difficulty:** Medium 
**Flag Format:** `Fl4g-X{latitude,longitude}`  
**Flag:** `Fl4g-X{10.03,76.30}`

### Challenge Description
The train glides along a gentle curve before reaching a small station surrounded by palms and shimmering backwaters. The humid breeze carries the scent of the coast,. Somewhere here, rails cross paths near a bustling junction. Can you spot this stop?

### Solution
1. Carefully reading the challenge description, phrases such as “palms and backwaters” and “the scent of the coast” act as strong geographical clues. These hints suggest a location rich in natural scenery and coastal features. A logical inference is Kerala, which is widely known for its backwaters and lush landscapes.
2. Upon opening the provided video, we observe a railway station with multiple tracks. A closer inspection shows that it is a small station and appears to be under construction, which helps narrow down potential locations.
3. To proceed, we use a trial-and-error approach, focusing on small railway stations in Kerala that have three railway tracks. During the CTF, an additional hint was released stating that the station lies on a Hyderabad to Kerala railway route, which significantly reduces the search space and makes the process easier.
4. After comparing multiple stations based on these criteria, we identify Idappally Railway Station, Kerala as it closely matches the visual details from the video and aligns with the location shown in the video.

---

## Happy Hacking!!