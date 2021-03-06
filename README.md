# InvitationNFT
I want to create an NFT which is going to be used as an invitation ticket.
This NFT should have same properties of a collectible, except that it shall not be transferable.
This means that the NFT shall be initially sent to some addresses, which are going to be called the "origins".

It will be integrated in the ZION dAPP suite (!! =) ) and it shall become deployable by anyone who already have a ZION invite NFT.

The use cases for this NFT are going to be this: <br>
1 - Permissioning addresses to access certain web3 content. <br>
2 - create sort of multi-level access scheme, giving possibility to leverage a referral scheme. <br>
3 - prevent malicious users by granting access to directly inviting people. <br>
4 - represent a badge, so basically as a swag tool. <br>
5 - Limit the numbers of founders based on some datas that can be retrived thanks to this badge (level height, usage of the miniting. <br>

Here the functions that should be implemented:

1 - choose how many "origin" addresses (this shall create a limited length array of addresses) <br>
2 - mint option for those who already have, which will be done by inserting the recipient address <br>
3 - counter of all the NFT created <br>
4 - counter of the tokens generated by the conncected address <br>
5 - counters of the tokens who actually performed certain requirements (participate in the crowdfuning, buy platform tokens etc..) <br>
6 - counter that will count how many tokens have been generated by the tokens invited by the connected token <br>
7 - dependencies cutter, which will cut one level of connection, making it be able to create a less pyramidal structure as time passes by* <br>

Here under a list of special function that shall be granted just to the "origins" addresses, and which shall undergo a governance votation:

1 - pause minting <br>
2 - restart minting <br>
3 - burn unused tokens who are older than 3 days (tokens which didnt log into the dAPP and tokens which logged but didnt performe the required action <br>

*the dependency cutter can be either a timebomb or a kill button.

# Front End Version v0.0
I just started out using the Open Zeppelin files.
I woul like to make this contract as light weight as possible to minimize users deployment gas fees, I actually still don't know how to do this, but I know it is possible!!

The first test version will be deployd on the the Goerli Test net.

The front end will prompt a logo in the homepage, and a connect metamask dialog box.
On the bottom of the page we will prompt logos of the partners (TNL, Plum Music, Psychoquake, Astrofonik, ..)
Users who will not own a token will just keep on seeing the logo.
Users who own an invitation token will be able to access the page and send out invitation.
Simple as that.... =)

You can see the design for this page here https://www.figma.com/file/Iwd71DyO47YhiOUmLP1M1Q/Invitation-NFT?node-id=1%3A41
