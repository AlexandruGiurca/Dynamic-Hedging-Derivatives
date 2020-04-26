### Dynamic Hedging Strategy that Replicates the Payoff of Different Derivatives

Implementation of a **dynamic, self-financing hedging strategy** that replicates the payoff of certain derivatives. The replicating strategy will be rebalanced ![$ N $](https://render.githubusercontent.com/render/math?math=%24%20N%20%24) times (including the initial portfolio).

The simulation is performed for the following payoffs,with ![$ K $](https://render.githubusercontent.com/render/math?math=%24%20K%20%24) being the option Strike.
- ![$V(T, S_T)=ln(S_T)$](https://render.githubusercontent.com/render/math?math=%24V(T%2C%20S_T)%3Dln(S_T)%24)
- ![$V(T, S_T)=(ln(S_T))^2$](https://render.githubusercontent.com/render/math?math=%24V(T%2C%20S_T)%3D(ln(S_T))%5E2%24)
- ![$V(T, S_T)=(S_T-K)^2$](https://render.githubusercontent.com/render/math?math=%24V(T%2C%20S_T)%3D(S_T-K)%5E2%24)
- ![$V(T, S_T)=\mathbf{1}_{S_T > K}$](https://render.githubusercontent.com/render/math?math=%24V(T%2C%20S_T)%3D%5Cmathbf%7B1%7D_%7BS_T%20%3E%20K%7D%24)
- ![$V(T, S_T)=max(S_T-K, 0)$](https://render.githubusercontent.com/render/math?math=%24V(T%2C%20S_T)%3Dmax(S_T-K%2C%200)%24)

When implementing the replication strategy Euler's method is used to discretize the price dynamics of the underlying asset. 
