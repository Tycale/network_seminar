# Network seminar

## Feedback

### Lessons learned
* To improve:
    - Advantage of websockets over simple TCP. I suppose there are some, but they are never mentionned in the paper.

### Bibliography
* To improve:
    - Dates are sometimes missing. Reference [2], [6] and [10] are such examples. Citations [3] and [5] refers to an actual (and same) book. It may be better to adapt the citation to reflect this.

    - However, there are some dates missing in this bibliography for some papers which makes the freshness of these ones hard to check.

    - The bibliography seems quite complete: a quick search on Google Scholar didn't reveal any major paper missing from the bibliography. I could however spot two incompleteness in the way [6] and [10] are cited. To be constructive, here are the complete citation of those paper (+ bibtex entries if students want to use it in their paper):

    Skvorc, D., Horvat, M., & Srbljic, S. (2014, May). Performance evaluation of Websocket protocol for implementation of full-duplex web streams. In Information and Communication Technology, Electronics and Microelectronics (MIPRO), 2014 37th International Convention on (pp. 1003-1008). IEEE.

    @inproceedings{skvorc2014performance,
    title={Performance evaluation of Websocket protocol for implementation of full-duplex web streams},
    author={Skvorc, D and Horvat, Marko and Srbljic, S},
    booktitle={Information and Communication Technology, Electronics and Microelectronics (MIPRO), 2014 37th International Convention on},
    pages={1003--1008},
    year={2014},
    organization={IEEE}
    }

    Huang, L. S., Chen, E. Y., Barth, A., Rescorla, E., & Jackson, C. (2011). Talking to yourself for fun and profit. Proceedings of W2SP, 1-11.

    @article{huang2011talking,
    title={Talking to yourself for fun and profit},
    author={Huang, Lin-Shung and Chen, Eric Y and Barth, Adam and Rescorla, Eric and Jackson, Collin},
    journal={Proceedings of W2SP},
    pages={1--11},
    year={2011}
    }

    Apart from that, I found that this survey emphasized a little bit too much on [7] (Pimentel, Nickerson) and [8] (Argawal) since it even cites values for measurements. (I would have expected to get the idea from the measurement, not the exact value).

    - References 2, 6 and 10 are missing the date and origin of publication.


### Organisation and writing style
* To improve:
    - The organisation is quiet good. Maybe the XMLHttpRequest should not be given as much importance as the rest of the paper. Moreover, the section title "long polling version" should either be deleted or an adequate "periodic polling version" should be existant.
    - Writing style is quiet good. There are minor Enlgish mistakes. Citations should not be followed by "they".

    - Concerning the writing style, a suggestion would be the add some authors' name while citing a document which could make it easier to the reader to associate this document with the ones in the references.

    - My only grief regarding the writing style is the (too frequent) use of the pronoun "we" (impersonal construction would imho have been better). Because of this, in the introduction of section 4 (Performance of websockets) it felt as if the students made the experiments that are explained in later sections. That impression was corrected right away in the next subsection (4.1) but still that felt a little awkward. My simple proposal to fix this would be to simply rephrase the last sentences in that paragraph and avoid the use of the pronoun 'we'.

### Figures
* To improve:
    - Maybe the Figure 2 illustrating the Websocket packet structure is useless in terms of understanding the text.

    - I would however either drop figure 7 or 8 since they convey the same message (the overhead diminishes with the chunk size, hence the throughput increases when the chunk size increases).

    - Maybe also add a little bit more space between both parts of figure 5, to have a cleaner cut between each text.


### General
* To improve:
    - This survey adds, in some parts of the text, a confusion about the layer in which the WebSocket resides. Indeed, a comparison between an application layer protocol (WebSocket) and the transport layer (TCP) upon which it is built seems a little bit odd since there is no way the former one can be better than the latter one. Maybe additional information about why the comparison is done could help the reader. However, in other parts of the text, the distinction is clearly done.

    - Overall I found this paper a pleasant read, concise, clear and to-the-point. Should the authors want to further improve the quality of their paper, I would suggest them to spend less time detailing the measurements observed in [7] and [8] and maybe mention one or several implementations of the web socket protocol that are available nowadays (the most famous of which are NodeJS/ws and socket.io). If those implementations are not fully compliant with the RFC6455, I think it would also be worth mentioning.

    - One thing that could be clearer though is the advantage(s) of WebSockets compared to TCP, as the survey right now leads readers to believe that TCP is strictly superior.
