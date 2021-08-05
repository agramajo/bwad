# PlanetPay playground

## Version 1 without LP and automatic swap

BWAD based on examples/NotSafeMoon.sol

[contract testnet](https://testnet.bscscan.com/address/)

TLDR

When the normal user swaps bnb for safemoon, bnb is added to the pool and 
safemoon is removed. This is normal and will increase the price of safemoon.

When the normal user adds Liquidity to the pool, they add an equal value of 
safemoon and bnb to the pool. This is normal and doesn’t change the price of 
Safemoon.

When the safemoon contract itself adds Liquidity to the pool, the contract 
begins with only the safemoon collected from the Liquidity fee. The contract 
has no external source of BNB. The net result is an addition of only safemoon 
to the pool. This is bad. This breaks the Constant Product which is used to 
determine the price. This lowers the price of Safemoon.

[Read more](https://notsafemoon.com/new/public/docs/MoonCoinsTA.pdf)

## Swap

Both have some liquidity in [pancake testnet](https://pancake.kiemtienonline360.com/)

## MORE INFO

### SAFEMOON AUDITS

https://certik-public-assets.s3.amazonaws.com/CertiK+Audit+Report+for+SafeMoon.pdf

https://jovonni.medium.com/safe-moon-the-problems-revealed-by-certiks-audit-of-safemoon-aeb8060b9b29

https://investorplace.com/2021/05/safemoon-audit-9-things-to-know-about-the-safemoon-certik-findings/

### SECURITY

https://forum.openzeppelin.com/t/what-is-it-about-safemoon-swapandliquify-and-numtokensselltoaddtoliquidity/9192/18

