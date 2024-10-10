---
title: FAKE Disclosure of DoS due to disabled op_code
name: blog-disclose-disabled-opcode
id: en-blog-disclose-disabled-opcode
lang: en
type: advisory
layout: post

## If this is a new post, reset this counter to 1.
version: 1

## Only true if release announcement or security annoucement. English posts only
announcement: 1

excerpt: >
  FAKE: An attacker could crash a Bitcoin Core node by sending a transaction that included a disabled op_code
---

**FAKE Vulnerability Disclosure for Warnet games.**

With Bitcoin Core v95.0.0, attackers could send transactions to nodes that include disabled op_codes which could be used to remotely crash peers.

Vulnerable nodes have the user agent of `disabled-opcodes:95.0.0`

This issue is considered **CRITIAL** severity.

## Details

Bitcoin Core version `disabled-opcodes:95.0.0` will crash if it's sent a transaction that includes a disabled op_code (such as OP_CAT). This makes it susceptible to being DoSed.

## Attribution

This attack was independently discovered and reported to the Bitcoin Core project in September 2024 by the warnet development team.

## Timeline

* **October 5, 2024**: Nodes start executing the long-lost "OP_CAT" opcode, causing global feline panic.
* **October 7, 2024**: Investigation uncovers that disabled opcodes are rising from the dead, hungry for CPU brains.
* **October 11, 2024**: Team develops a "zombie opcode" vaccine using a mixture of garlic and thermal paste.
* **October 16, 2024**: Solution completed after an intense montage of developers training in opcode martial arts.
* **October 21, 2024**: Final testing conducted in an abandoned blockchain warehouse during a full moon.
* **October 23, 2024**: Vulnerability disclosed. Users must update while wearing zombie makeup and chanting "Brains... I mean, Blocks!"

{% include references.md %}
