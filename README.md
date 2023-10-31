# electrum-dash-dependencies
Binaries on which electrum-dash depends. 

The need to keep copies of some of the binaries on which the electrum-dash building process depends arose from the situation described here:
- https://gmplib.org/
> NEWS 2023-06-21: The GMP servers has been under serious load due to a barrage of clone requests from Microsoft/Github. Github's setup encourages "forks" of their projects, and such forks then by default pull in parent project changes. Around 2023-06-15, a project known as FFmpeg decided that it would be a great idea to clone GMP in their CI scripts, meaning that every one of their commits requested a compressed clone from the GMP servers. But, by Github's design, hundreds of FFmpeg forks automatically followed suit, themselves cloning the GMP repo.
>
> In effect, Microsoft's computer cloud performed a DDoS attack on the GMP servers.
>
> After bringing up the issue here and on the GMP mailing lists, some Github brass replied, minimizing the issue and blaming our servers for the denial-of-service attack. They did not do anything to stop the attack! In fact, it is still ongoing a week later.
>
> Our servers are fully available again, but that's the result of us adding all participating Microsoft network ranges to our firewall. We understand that we are far from the first project to take such measures against Github.
- https://github.com/microsoft/vcpkg/issues/33316
> GMP has blocked Microsoft's IP addresses since 21 June 2023, which means that trying to fetch the GMP tarball via vcpkg on a CI build fails.



