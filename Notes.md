# Notes

## Dissertation Outline

1. Introduction
2. Background on distributed storage networks (platforms)
 * NFS's (relates to how I am using the SAFE network)
 * The 'serverless' architecture model
 * Highlight other systems we will use to compare SAFE against
3. SAFE Network
 * The differences it has with conventional systems
 * Self encryption
 * File chunking
 * Fault tolerance
 * Make sure to highlight exactly how the SAFE network differs from other systems
4. My application
 * What is is and the motivation for it
 * Why it would benefit from being on the SAFE Network and a 'serverless' architecture
 * How it benefits from using the SAFE network rather than other systems
 * NFS
5. Critical analysis/critique of a performance measure in relation to other distributed storage networks.
 * Relate SAFE back to other systems that exist
 * Highlight where SAFE is clearly better
 * Highlight where SAFE isn't better than other systems
6. Conclusion

## Potential Performance Measures

What critical performance measures we examine depends greatly on the abilities that the SAFE network currently has. Since the network is only in Alpha 2, it becomes difficult to accurately critique some of the technical aspects of the system.

One thing we could examine is the distribution of the network in relation to other solutions. I am not entirely sure that the current [safe_vault](https://github.com/maidsafe/safe_vault) implementation is capable or far enough advanced to accurately examine the distributed nature of the network. It may be possible, but results gathered may become useless/outdated very quickly. Alpha 3 should bring big changes to this when it is fully released sometime next year.

If the [safe_vault](https://github.com/maidsafe/safe_vault) is capable, I propose exploring the random access performance of the network. By examining this, it becomes possible to compare it to other distributed storage networks and gives us a clear avenue to critique the network if it doesn't hold up as well as it should. Specifically, this could be a comparison to other distributed NFS's. It could be possible to explore the 'why/how' to our values, and explain tradeoffs with performance and other factors.  The success of the SAFE network hinges a lot on this metric, people will not use it if it is too slow.

Throughout the dissertation, it will be very important to keep reiterating that this is very early on in development of the SAFE Network. Performance may increase, or decrease, as it nears full release and more features are added.
