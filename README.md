# Preparing the Docker Containers

In order to run the challenge POCs without any problem, I prepared docker containers for various Ubuntu releases. The instructions for using the containers can be found [here](docker).

# Writeups

| CTF                        | Challenge   | Info               | Exploitation         |
|:--------------------------:|:-----------:|--------------------|----------------------|
| [UTCTF<br>2019](UTCTF/2019)| [BabyEcho](UTCTF/2019/BabyEcho) | `x86_32`<br>`Partial RELRO`<br>`ASLR`<br>`NX` | `format string`<br>`GOT`<br>`libc database` | [CTFtime Event](https://ctftime.org/event/757) |
| [BSidesSF<br>2019](BSidesSF/2019)| [slowfire](BSidesSF/2019/slowfire) | `x86_64`<br>`Partial RELRO`<br>`ASLR` | `stack overflow`<br>`shellcode`<br>`syscall`<br>`socket`<br>`GOT`<br>`PLT`  | [CTFtime Event](https://ctftime.org/event/753) |
| [TAMUctf<br>2019](TAMUctf/2019)| [pwn3](TAMUctf/2019/pwn3) | `x86_32`<br>`Full RELRO`<br>`PIE`<br>`ASLR` | `stack overflow`<br>`shellcode`<br>`syscall` | [CTFtime Event](https://ctftime.org/event/740) |
| [TAMUctf<br>2019](TAMUctf/2019)| [pwn5](TAMUctf/2019/pwn5) | `x86_32`<br>`Partial RELRO`<br>`NX`<br>`ASLR` | `stack overflow`<br>`ret2libc` | [CTFtime Event](https://ctftime.org/event/740) |
| [ASIS<br>2018 Finals](ASIS/2018/Finals)| [asvdb](ASIS/2018/Finals/asvdb) | `x86_64`<br>`NX`<br>`Canary`<br>`ASLR`<br>`Full RELRO` | `heap`<br>`tcache`<br>`use after free`<br>`double free`<br>`unsorted bin`<br>`smallbin`<br>`tcache dup`<br>`tcache poisoning`<br>`__free_hook`<br>`one gadget` | [CTFtime Event](https://ctftime.org/event/620) |
| [ASIS<br>2018 Finals](ASIS/2018/Finals)| [inception](ASIS/2018/Finals/inception) | `x86_64`<br>`Partial RELRO`<br>`NX`<br>`ASLR` | `stack overflow`<br>`ROP`<br>`GOT`<br>`one gadget`<br>`pipe`<br>`fork`<br>`return-to-csu` | [CTFtime Event](https://ctftime.org/event/620) |
| [SECCON<br>2018](SECCON/2018)| [profile](SECCON/2018/profile) | `x86_64`<br>`NX`<br>`Canary`<br>`ASLR`<br>`Partial RELRO` | `buffer overflow`<br>`C++`<br>`GOT`<br>`arbitrary read`<br>`string`<br>`one gadget` | [CTFtime Event](https://ctftime.org/event/683) |
| [SECCON<br>2018](SECCON/2018)| [classic](SECCON/2018/classic) | `x86_64`<br>`NX`<br>`ASLR`<br>`Partial RELRO` | `stack overflow`<br>`ROP`<br>`GOT`<br>`stack pivoting`<br>`one gadget` | [CTFtime Event](https://ctftime.org/event/683) |
| [BSidesDelhi<br>2018](BSidesDelhi/2018)| [data_bank](BSidesDelhi/2018/data_bank) | `x86_64`<br>`NX`<br>`Canary`<br>`ASLR`<br>`Full RELRO`<br>`PIE` | `heap`<br>`tcache`<br>`use after free`<br>`tcache poisoning`<br>`__malloc_hook`<br>`one gadget` | [CTFtime Event](https://ctftime.org/event/700) |
| [HITCON<br>2018](HITCON/2018)| [children_tcache](HITCON/2018/children_tcache) | `x86_64`<br>`NX`<br>`Canary`<br>`ASLR`<br>`Full RELRO`<br>`PIE` | `heap`<br>`tcache`<br>`off-by-one`<br>`poison-null-byte`<br>`double free`<br>`overlapping chunks`<br>`tcache dup`<br>`tcache poisoning`<br>`__malloc_hook` | [CTFtime Event](https://ctftime.org/event/669) |
| [Hack.lu<br>2018](Hack.lu/2018)| [BabyPHP](Hack.lu/2018/BabyPHP) | `Web`<br>`PHP` | `unsanitized input`<br>`unintended behaviors`<br>`code injection`<br>`assert` | [CTFtime Event](https://ctftime.org/event/699) |
| [InCTF<br>2018](InCTF/2018)| [wARMup](InCTF/2018/wARMup) | `armhf`<br>`arm32`<br>`ARM`<br>`Partial RELRO`<br>`ASLR` | `stack overflow`<br>`shellcode`<br>`syscall` | [CTFtime Event](https://ctftime.org/event/662) |
| [InCTF<br>2018](InCTF/2018)| [YAWN](InCTF/2018/YAWN) | `x86_64`<br>`NX`<br>`Canary`<br>`ASLR`<br>`Full RELRO` | `heap`<br>`off-by-one`<br>`fastbin dup`<br>`__malloc_hook`<br>`one gadget`<br>`GOT` | [CTFtime Event](https://ctftime.org/event/662) |
| [InCTF<br>2018](InCTF/2018)| [securepad](InCTF/2018/securepad) | `x86_64`<br>`NX`<br>`Canary`<br>`ASLR`<br>`Full RELRO`<br>`PIE` | `heap`<br>`uninitialized var`<br>`arbitrary free`<br>`unsorted bin`<br>`fastbin dup`<br>`__free_hook` | [CTFtime Event](https://ctftime.org/event/662) |
| [CSAW<br>2018 Quals](CSAW/2018/Quals)| [alien_invasion](CSAW/2018/Quals/alien_invasion) | `x86_64`<br>`NX`<br>`Canary`<br>`ASLR`<br>`Partial RELRO`<br>`PIE` | `heap`<br>`off-by-one`<br>`poison-null-byte`<br>`overlapping chunks`<br>`GOT` | [CTFtime Event](https://ctftime.org/event/633) |
| [CSAW<br>2018 Quals](CSAW/2018/Quals)| [bigboy](CSAW/2018/Quals/bigboy) | `x86_64`<br>`NX`<br>`Canary`<br>`ASLR`<br>`Partial RELRO` | `stack overflow` | [CTFtime Event](https://ctftime.org/event/633) |
| [CSAW<br>2018 Quals](CSAW/2018/Quals)| [get_it](CSAW/2018/Quals/get_it) | `x86_64`<br>`NX`<br>`ASLR`<br>`Partial RELRO` | `stack overflow` | [CTFtime Event](https://ctftime.org/event/633) |
| [CSAW<br>2018 Quals](CSAW/2018/Quals)| [shell_code](CSAW/2018/Quals/shell_code) | `x86_64`<br>`ASLR`<br>`Full RELRO`<br>`PIE` | `stack overflow`<br>`shellcode` | [CTFtime Event](https://ctftime.org/event/633) |
| [WhiteHatGrandPrix<br>2018 Quals](WhiteHatGrandPrix/2018/Quals)| [pwn02](WhiteHatGrandPrix/2018/Quals/pwn02) | `x86_64`<br>`NX`<br>`Canary`<br>`ASLR`<br>`Full RELRO`<br>`FORTIFY` | `heap`<br>`off-by-one`<br>`poison-null-byte`<br>`overlapping chunks`<br>`glibc tcache` | [CTFtime Event](https://ctftime.org/event/656) |
| [MeePwn<br>2018 Quals](MeePwn/2018/Quals)| [BabySandbox](MeePwn/2018/Quals/BabySandbox) | `x86_32`<br>`Partial RELRO`<br>`ASLR`<br>`NX`<br>`PIE` | `shellcode`<br>`syscall`<br>`openat`<br>`readv`<br>`writev`<br>`socket` | [CTFtime Event](https://ctftime.org/event/625) |
| [0CTF<br>2018 Finals](0CTF/2018/Finals)| [freenote2018](0CTF/2018/Finals/freenote2018) | `x86_64`<br>`NX`<br>`Canary`<br>`PIE`<br>`Full RELRO`<br>`ASLR` | `heap`<br>`double free`<br>`overlapping chunks`<br>`heap metadata`<br>`__malloc_hook`<br>`fastbin dup` | [CTFtime Event](https://ctftime.org/event/558) |
| [RCTF<br>2018](RCTF/2018)| [RNote3](RCTF/2018/RNote3) | `x86_64`<br>`NX`<br>`Canary`<br>`PIE`<br>`Full RELRO`<br>`ASLR` | `uninitialized var`<br>`heap`<br>`overlapping chunks`<br>`one gadget`<br>`fastbin`<br>`__free_hook` | [CTFtime Event](https://ctftime.org/event/624) |
| [RCTF<br>2018](RCTF/2018)| [babyheap](RCTF/2018/babyheap) | `x86_64`<br>`NX`<br>`Canary`<br>`PIE`<br>`Full RELRO`<br>`ASLR` | `heap`<br>`off-by-one`<br>`poison-null-byte`<br>`__malloc_hook`<br>`PREV_IN_USE bit` | [CTFtime Event](https://ctftime.org/event/624) |
| [RCTF<br>2018](RCTF/2018)| [stringer](RCTF/2018/stringer) | `x86_64`<br>`NX`<br>`Canary`<br>`PIE`<br>`Full RELRO`<br>`ASLR` | `heap`<br>`off-by-one`<br>`IS_MMAPED`<br>`calloc`<br>`double free`<br>`fastbin dup`<br>`__malloc_hook` | [CTFtime Event](https://ctftime.org/event/624) |
| [PlaidCTF<br>2018](PlaidCTF/2018)| [shop](PlaidCTF/2018/shop) | `x86_64`<br>`NX`<br>`Canary`<br>`Partial RELRO`<br>`ASLR` | `heap`<br>`buffer overflow`<br>`one gadget`<br>`GOT` | [CTFtime Event](https://ctftime.org/event/617) |
| [ASIS<br>2018 Quals](ASIS/2018/Quals)| [Cat](ASIS/2018/Quals/Cat) | `x86_64`<br>`NX`<br>`Canary`<br>`Partial RELRO`<br>`ASLR` | `heap`<br>`fastbin`<br>`GOT` | [CTFtime Event](https://ctftime.org/event/568) |
| [ASIS<br>2018 Quals](ASIS/2018/Quals)| [FiftyDollars](ASIS/2018/Quals/FiftyDollars) | `x86_64`<br>`NX`<br>`Canary`<br>`PIE`<br>`Full RELRO`<br>`ASLR` | `heap`<br>`use after free`<br>`double free`<br>`fastbin` | [CTFtime Event](https://ctftime.org/event/568) |
| [ASIS<br>2018 Quals](ASIS/2018/Quals)| [JustSort](ASIS/2018/Quals/JustSort) | `x86_64`<br>`NX`<br>`Canary`<br>`Partial RELRO`<br>`ASLR` | `heap overflow`<br>`GOT`<br>`one gadget` | [CTFtime Event](https://ctftime.org/event/568) |
| [ASIS<br>2018 Quals](ASIS/2018/Quals)| [MessageMe](ASIS/2018/Quals/MessageMe) | `x86_64`<br>`NX`<br>`Canary`<br>`Partial RELRO`<br>`ASLR` | `heap`<br>`use after free`<br>`double free`<br>`fastbins`<br>`__malloc_hook`<br>`overlapping chunks` | [CTFtime Event](https://ctftime.org/event/568) |
| [StarCTF<br>2018](StarCTF/2018)| [babystack](StarCTF/2018/babystack) | `x86_64`<br>`NX`<br>`Canary`<br>`Full RELRO`<br>`ASLR` | `stack overflow`<br>`GOT`<br>`pthread`<br>`thread local storage`<br>`stack_guard` | [CTFtime Event](https://ctftime.org/event/614/) |
| [StarCTF<br>2018](StarCTF/2018)| [note](StarCTF/2018/note) | `x86_64`<br>`NX`<br>`Full RELRO`<br>`ASLR` | `stack overflow`<br>`off-by-one`<br>`ROP`<br>`LSB`<br>`saved rbp`<br>`GOT` | [CTFtime Event](https://ctftime.org/event/614/) |
| [StarCTF<br>2018](StarCTF/2018)| [warmup](StarCTF/2018/warmup) | `x86_64`<br>`NX`<br>`Full RELRO`<br>`ASLR` | `stack overflow`<br>`one gadget`<br>`GOT` | [CTFtime Event](https://ctftime.org/event/614/) |
| [WPICTF<br>2018](WPICTF/2018)| [ForkerLevel1](WPICTF/2018/ForkerLevel1) | `x86_64`<br>`Partial RELRO`<br>`ASLR` | `stack overflow`<br>`return-to-csu`<br>`ROP`<br>`GOT`<br>`shellcode` | [CTFtime Event](https://ctftime.org/event/600) |
| [WPICTF<br>2018](WPICTF/2018)| [ForkerLevel2](WPICTF/2018/ForkerLevel2) | `x86_64`<br>`NX`<br>`Canary`<br>`Partial RELRO`<br>`ASLR` | `stack overflow`<br>`stack canary`<br>`stack cookie`<br>`fork`<br>`socket` | [CTFtime Event](https://ctftime.org/event/600) |
| [UIUCTF<br>2018](UIUCTF/2018)| [how2heap](UIUCTF/2018/how2heap) | `x86_64`<br>`NX`<br>`Canary`<br>`PIE`<br>`Full RELRO`<br>`ASLR` | `heap`<br>`one gadget` | [CTFtime Event](https://ctftime.org/event/587) |
| [0CTF<br>2018 Quals](0CTF/2018/Quals)| [babyheap](0CTF/2018/Quals/babyheap) | `x86_64`<br>`NX`<br>`Canary`<br>`PIE`<br>`Full RELRO`<br>`ASLR` | `heap`<br>`off-by-one`<br>`double free`<br>`fastbin dup`<br>`__malloc_hook`<br>`one gadget`<br>`top chunk` | [CTFtime Event](https://ctftime.org/event/557) |
| [0CTF<br>2018 Quals](0CTF/2018/Quals)| [babystack](0CTF/2018/Quals/babystack) | `x86_32`<br>`Partial RELRO`<br>`ASLR`<br>`NX` | `stack overflow`<br>`ROP`<br>`GOT`<br>`PLT`<br>`Elf_Rel`<br>`Elf_Sym`<br>`dynstr`<br>`dynsym`<br>`rel_plt` | [CTFtime Event](https://ctftime.org/event/557) |
| [iCTF<br>2018](iCTF/2018)| [fantasticiot](iCTF/2018/fantasticiot) | `x86_32`<br>`Canary`<br>`NX`<br>`ASLR` | `attack & defense`<br>`strncmp`<br>`binary patching` | [CTFtime Event](https://ctftime.org/event/567) |
| [TAMUctf<br>2018](TAMUctf/2018)| [pwn5](TAMUctf/2018/pwn5) | `x86_32`<br>`Partial RELRO`<br>`NX`<br>`ASLR` | `stack overflow`<br>`ROP`<br>`syscall` | [CTFtime Event](https://ctftime.org/event/559) |
| [NullconHackIM<br>2018](NullconHackIM/2018)| [pwn2-box](NullconHackIM/2018/pwn2-box) | `x86_64`<br>`Partial RELRO`<br>`ASLR` | `shellcode`<br>`ROP`<br>`one gadget`<br>`syscall` | [CTFtime Event](https://ctftime.org/event/566) |
| [Codegate<br>2018](Codegate/2018)| [BaskinRobins31](Codegate/2018/BaskinRobins31) | `x86_64`<br>`Partial RELRO`<br>`NX`<br>`ASLR` | `stack overflow`<br>`ROP`<br>`GOT`<br>`one gadget`<br>`stack pivot` | [CTFtime Event](https://ctftime.org/event/542) |
| [Codegate<br>2018](Codegate/2018)| [SuperMarimo](Codegate/2018/SuperMarimo) | `x86_64`<br>`Canary`<br>`Partial RELRO`<br>`NX`<br>`ASLR` | `heap`<br>`GOT`<br>`fastbin`<br>`one gadget` | [CTFtime Event](https://ctftime.org/event/542) |
| [0CTF<br>2017 Quals](0CTF/2017/Quals)| [babyheap](0CTF/2017/Quals/babyheap) | `x86_64`<br>`NX`<br>`Canary`<br>`PIE`<br>`Full RELRO`<br>`ASLR` | `heap overflow`<br>`fastbin`<br>`smallbin`<br>`IS_MMAPED`<br>`calloc`<br>`fastbin attack`<br>`__malloc_hook`<br>`one gadget` | [CTFtime Event](https://ctftime.org/event/402) |
| [C3CTF<br>2017](C3CTF/2017)| [SimpleGC](C3CTF/2017/SimpleGC) | `x86_64`<br>`Canary`<br>`Partial RELRO`<br>`NX`<br>`ASLR` | `heap`<br>`use after free`<br>`GOT`<br>`glibc tcache`<br>`fastbin` | [CTFtime Event](https://ctftime.org/event/544) |
| [SECCON<br>2017](SECCON/2017)| [election](SECCON/2017/election) | `x86_64`<br>`Canary`<br>`Full RELRO`<br>`NX`<br>`ASLR` | `null byte poisoning`<br>`off-by-one`<br>`null byte overflow`<br>`GOT`<br>`__malloc_hook`<br>`one gadget`<br>`fastbin` | [CTFtime Event](https://ctftime.org/event/512) |
| [SECCON<br>2017](SECCON/2017)| [secure_keymanager](SECCON/2017/secure_keymanager) | `x86_64`<br>`Canary`<br>`Partial RELRO`<br>`NX`<br>`ASLR` | `heap`<br>`double free`<br>`format string`<br>`GOT`<br>`PLT`<br>`fastbin` | [CTFtime Event](https://ctftime.org/event/512) |
| [SECCON<br>2017](SECCON/2017)| [video_player](SECCON/2017/video_player) | `x86_64`<br>`Canary`<br>`Partial RELRO`<br>`NX`<br>`ASLR` | `heap`<br>`use after free`<br>`GOT`<br>`one gadget`<br>`__malloc_hook`<br>`vtable`<br>`virtual calls`<br>`overlapping chunks`<br>`fastbin` | [CTFtime Event](https://ctftime.org/event/512) |
| [CSAW<br>2017 Quals](CSAW/2017/Quals)| [SCV](CSAW/2017/Quals/SCV) | `x86_64`<br>`Canary`<br>`Partial RELRO`<br>`NX`<br>`ASLR` | `stack overflow`<br>`buffer overflow`<br>`information disclosure`<br>`buffer over-read`<br>`ROP`<br>`one gadget` | [CTFtime Event](https://ctftime.org/event/488) |
