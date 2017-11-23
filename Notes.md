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

Due to the upcoming features in Alpha 3, I have found it difficult to pin-point something to critically analyse. My main worry is that I research something that becomes invalid/outdated when Alpha 3 (and beyond) is released. So any suggestions on what I could explore would be greatly appreciated.

The first idea I had was to look in depth at the distribution/decentralised aspect of the network. This would involve running a few [safe_vault's](https://github.com/maidsafe/safe_vault) and gathering any test data (metrics) needed. As changes coming in Alpha3 seem to be covering these aspects specifically, I feel that any research or findings I come up with could quickly become invalidated.

The best idea I have came up with so far is to study the performance of NFS. With my program, I am planning on storing large files on the network. When the current file size limit is lifted these files could be as large as 60+ GB. With the NFS support you currently have in the Node api, I am planning on using File.read() to read the parts of the file I need when required. As far as I understand, this can simply 'stream' the data that is asked for and avoid having to fetch the entire file. This will be random access, which I think would be interesting to compare against the performance of sequential reads from the network. From this I can further elaborate and explore other performance measures that we find interesting to study. For further context, I am adapting [kiwix-js](https://github.com/kiwix/kiwix-js) to use the SAFE network for the retrieval of zim files. This essentially means that it is easy to serve mirrors of websites like Wikipedia on the SAFE Network. So far I have managed to bundle kiwix-js into an Electron app, and have just started integration with the SAFE Network.
