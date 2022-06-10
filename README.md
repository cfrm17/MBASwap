# MBA Swap

The BMA Municipal Swap Index, produced by Municipal Market Data (MMD), is a single rate released every and effective on next business date. The rate is a representative index made up of an average of rates supplied by traders within the industry. In a generic fixed for floating BMA swap, the floating side is estimated using averages of weekly BMA Municipal Swap Index.

While actual par Municipal Swap Rates are not available in the market, BMA ratios, which are actively traded, are applied to LIBOR par swap rates to derive the par BMA swap rate. BMA ratios are used in conjunction with LIBOR swap rates to calculate the various instruments traded in the BMA market.

In a generic fixed for floating BMA swap, the floating side is estimated using averages of the BMA Municipal Swap Index, which is published on a weekly basis. The fixed side pays interest quarterly on a 30/360 yield basis and payment dates adjusted using modified following basis. The floating side pays interest quarterly in ACT/ACT yield basis and payment dates adjusted using the modified following basis.

Three types of swap legs are available, including BMA leg as well as typical LIBOR (floating) leg and fixed leg with variable notional. BMA leg pays (or receives) weighted average of weekly BMA indices over specified periods, based on ACT/ACT day count basis (DCB). LIBOR leg receives (or pay) LIBOR rate multiplied by a fixed ratio using ACT/360 DCB.

BMA CMS swap is composed of BMA leg and BMA CMS leg. BMA CMS leg pays weighted average of CMS rates, calculated weekly, over payment periods and the CMS rates are forward BMA swap rates calculated as weighted average of weekly BMA rates over 3-month periods with CMS tenor. 

For convexity and timing value calculation for CMS rates, Hull-White formula with correlation coefficient set at 0.7 is used. This methodology requires heavy computation since CMS rates need to be calculated weekly (for 20 year BMA CMS leg requires over 1,000 CMS rate calculations). To improve the computation performance. 

The BMA Municipal Swap Index is a 7-day high-grade market index comprised of tax-exempt VRDNs from MMD’s extensive database. The rate is a representative index made up of an average of rates supplied by traders within the industry.

It is a simple annual rate with the day count convention (DCC) of ACT/ACT. Spot BMA rates are reset at every business Wednesday after 4:00 pm and effective on next business date (usually Thursday) and matures on next business Wednesday inclusive with a holiday adjustment based on the holiday centre of “NYC” and day roll convention (DRC) of “Following”.

If a Wednesday is not a good business day, the BMA reset day rolls over to next business day with the holiday of “NYC” and the DRC of “Following”. Then, the BMA rate is effective on the reset day and also matures on next business Wednesday inclusive with a holiday adjustment based on the holiday centre of “NYC” and DRC of “Following”.

While actual par Municipal Swap Rates are not available in the market, BMA ratios, which are actively traded, are applied to LIBOR par swap rates to derive the par BMA swap rate. BMA ratios are quoted for terms 3M, 1, 2Y, 3Y, 4Y, 5Y, 7Y, 10Y, 12Y, 15Y, 20Y, 30Y, 40Y in the BMA market. These quotes are used in conjunction with LIBOR swap rates to calculate the various instruments traded in the BMA market.

References:

https://finpricing.com/lib/EqVariance.html

https://zenodo.org/record/6558053/files/MbaSwap.pdf

https://zenodo.org/record/6558053#.YpDwC6gpDq4




