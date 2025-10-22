# CTF-write-ups---TryHackMe-Corridor
A simple write-ups about TryHackMe Challenge

## Challenge Information
- **Platform**: TryHackMe
- **Room**: Corridor
- **Difficulty**: Easy
- **Category**: Web Security, IDOR

## Objective
Find the flag by exploiting an IDOR vulnerability using predictable MD5 hashes.

## Methodology
1. Navigated through the corridor doors
2. Noticed URL pattern: `http://<IP>/s<md5-hash>`
3. Cracked hashes using CrackStation (found numbers 1-13)
4. Missing door 0 → hashed '0' to get `cfcd208495d565ef66e7dff9f98764da`
5. Accessed the missing door and found the flag

## Tools Used
- CrackStation
- CyberChef
- Browser DevTools
