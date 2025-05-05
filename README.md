# Crypto-Analysis

I created this project to help me test my hypothesis on the correlation between certain cryptocurrencies or rather groups of cryptocurrencies on 12 hour intervals to then apply the results to real life trading of crypto perpetual futures contracts. 

The program fetches historical price data using the Binance and Kucoin APIs (I used two just to see the differences, but you could stick to just one). Then it filters days where Primary Token's price changes by more than 1% (delta>0.01) at the close of t_0. For these filtered days, it evaluates whether Secondary Token’s price at the close of t_1 was higher than its price at t_0, or whether Secondary Token’s price at t_1 was lower than its price at t_0 when BTC’s price decreased by more than 1%. The results are presented as success rates for these scenarios.

This project was a great practice and introduciton to algorithmic trading. A few pairs performed pretty well in testing, then perhaps move over to Trading View and put a few technical indicators on top to filter it out even more and then lastly write a code in Pine Script that will notify me whenever the conditions are triggered.
