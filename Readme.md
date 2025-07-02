### Symmetric matrix: Wigner, Wishart

- **Francis Bach, 2023,** https://arxiv.org/abs/2303.01372
    - Derivation of Silverstein equation in Appendix A. Very clean and intuitive derivation (Woodbury + leave one out approach). Have the same spirit as the Silverstein 1995 paper, but much easier to follow.
    - Nice derivation of two point equivalence using similar leave one out method.
    - Catalogue the known asymptotic results for double descent for regression.
- **Alex, Jacob, Cengiz, 2024, Scaling and renormalization in high-dimensional regression** https://arxiv.org/abs/2405.00592  ***
    - Very elegant exposition of the Free probability approach for deriving the self-consistent equation (Sec. II-IV) and deterministic equivalence for empirical covariance matrix. and they used it for regression theory (Sec. V).
- Jacob 2024, Lecture note https://jzv.io/assets/pdf/am226_generalization_in_ridge_regression_lecture_notes.pdf
    - a simpler and shorter version of the review above.
- **Alex Blake Jacob et al. 2025** Two point deterministic equivalence and its application in linear regression
    - https://arxiv.org/abs/2408.04607
    - https://arxiv.org/abs/2502.05074
    - Most notes above just relied on one point equivalence, this result goes beyond that.
- **Geoff Pleiss, Topics in Deep Learning Theory  (stat547u)**  
https://geoffpleiss.com/teaching/stat547u/
    - Geoff Pleiss’s nice and fast RMT Intro. https://geoffpleiss.com/static/media/stat547u_lecture04.2af15a85.pdf
        - Introduced for computing spectrum and properties for Ridge Regression, covering Silverstein equation. (though the derivation of Silverstein is a bit jumpy.)
- **Pennington et al. RMT tutorial at ICML 2021** 
https://random-matrix-learning.github.io/
    - Part II mentioned some derivation of MP law and Silverstein equation (*the Woodbury approach*), but still quite jumpy… 
    https://random-matrix-learning.github.io/#presentation2
- **Ryan Tibshirani, Advanced Topics in Statistical Learning (stat241B)**
https://www.stat.berkeley.edu/~ryantibs/statlearn-s23/
    - Very nice note covering the theory for Ridge and Ridgeless case. ***
    https://www.stat.berkeley.edu/~ryantibs/statlearn-s23/lectures/ridge.pdf
    https://www.stat.berkeley.edu/~ryantibs/statlearn-s23/lectures/ridgeless.pdf
        - In the Ridge case, nicely stated the RMT approach and the known results for Ridge regression (though the Silverstein and MP results were cited instead of derived.)
- **Song Mei, Mean Field Asymptotics in Statistical Learning (STAT260)**
https://www.stat.berkeley.edu/~songmei/Teaching/STAT260_Spring2021/schedule.html
    - Note on random matrices and Stieltjes transforms, ***
    https://www.stat.berkeley.edu/~songmei/Teaching/STAT260_Spring2021/Lecture_notes/scribe_lecture17.pdf
        - Very comprehensively cataloguing many known properties of Stieltjes. Very detailed in covering the derivation of Semicircle law of **Wigner matrix**, using Schur complement + leave one out approach.
    - Note on Replica method for GOE+spike, derivation of BBP phase transition. 
    https://www.stat.berkeley.edu/~songmei/Teaching/STAT260_Spring2021/Lecture_notes/scribe_lecture8.pdf 
    https://www.stat.berkeley.edu/~songmei/Teaching/STAT260_Spring2021/Lecture_notes/scribe_lecture9.pdf
- **Laszlo Erdos, The matrix Dyson equation** 
https://arxiv.org/abs/1903.10060
    - Nice derivation of the **Wigner** semicircle law in Sec. 3, (using resolvent, leave-one-out and Schur complement approach). The author mentioned this as a special case of the matrix Dyson equation, i.e. scalar Dyson equation.
- Recent blog on spectral density empirical covariance with power-law population spectrum 
https://aaronjhf.github.io/blog/power-law-spec/
    - Code https://github.com/aaronjhf/Power-Law-Data
- Other classic works [*not recommended*]
    - Marcheko Pastur, 1967, [Russian version](https://www.mathnet.ru/links/a5682dd94bf93b80a69b1ee7be2bcf24/sm4101.pdf), [English version](https://www.mathnet.ru/links/9e89a7fa397dcc9991b34b3e52e0c462/sm4101_eng.pdf). Fundamental work, but a bit hard to read, due to notation differences… The derivation is more general than later works.
    - Silverstein, Bai et al. ~ 1995 seminal works, but the proofs are a bit hard to read due to notations and the results are distributed across a few papers …
        - [On the Empirical Distribution of Eigenvalues of a Class of Large Dimensional Random Matrices](https://www.sciencedirect.com/science/article/pii/S0047259X85710512) → self consistent equation for the kernel like matrix XTX*
        - [Strong Convergence of the Empirical Distribution of Eigenvalues of Large Dimensional Random Matrices](https://www.sciencedirect.com/science/article/pii/S0047259X85710834)  https://jack.math.ncsu.edu/strong.pdf → Silverstein equation, for the covariance like matrix XX*T. The leave one out approach is great, though the notation is not super clean …
        - Proof in their 2010 book is also not easy to read either …
    - Girko 1985 [Russian version](https://www.mathnet.ru/links/e7f5d8701907be00c25383266dde34e7/rm2141.pdf), [English version](https://www.mathnet.ru/links/04f444734b9fcba9066868a7a6b98cc7/rm2141_eng.pdf)
        - Generalize to non symmetric case

### Asymmetric matrix

- **Terence Tao 2010, RMT Teaching notes**
https://terrytao.wordpress.com/category/teaching/254a-random-matrices/
    - Esp. nice for the asymmetric non-Hermitian case, esp. Circular law https://terrytao.wordpress.com/2010/03/14/254a-notes-8-the-circular-law/
    - Using the Potential energy
- **Sommers & Haim 1988, Spectrum of Large Random Asymmetric Matrices** 
https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.60.1895  [**PDF link**](https://dspcsp.com/pubs/somcrisomste.pdf)
    - Classic seminal work on non-symmetric case using Greens function / Stieljes + Replica. Generalizing the circular law to the ellipse law when there is correlation between $J_{ij}$ and $J_{ji}$.
    - Mentioning the nice connection of Stieljes to the electric potential in 2d space.
- **Rajan & Abbott 2006, Random matrix with some all positive and all negative (exc and inh) columns**
https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.97.188104 
[**PDF link**](https://www.columbia.edu/cu/neurotheory/Larry/RajanPRL06.pdf)
Similar approach as above Greens function / Stieljes + Replica.