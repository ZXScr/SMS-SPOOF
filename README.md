Messages Gateway, send free messages all over Europe using SMTP/SMS exploit !

## Resources

We use the [K-framework] and its verification infrastructure throughout the formal verification effort.
All of the formal specifications are mechanized within the K-framework as well.
Therefore, some background knowledge about the K-framework would be necessary for reading and fully understanding the formal specifications and reproducing the mechanized proofs.
We refer the reader to the following resources for background knowledge about the K-framework and its verification infrastructure.

* [K-framework]
  * [Download] and [install]
  * [K tutorial]
  * [K editor support]
* [KEVM]: an executable formal semantics of the EVM in K
  * [Jellopaper]: reader-friendly formatting of KEVM
  * [KEVM research paper]
* [K reachability logic prover]
  * [eDSL]: domain-specific language for EVM-level specifications
* [ERC20-K]: a formal specification of the high-level business logic of [ERC20]
* [ERC20-EVM]: an EVM-level refinement of ERC20-K
* [ERC777-K]: a formal specification of the high-level business logic of [ERC777]

## License

Copyrightable work in this repository is licensed by Runtime Verification, Inc. under the terms of [The Reproducibility License 1.1.0](/LICENSE.md), a restrictive license.  That license is very readable, and you should read it.  Most will want to pay special attention to its [Reproducibility section](./LICENSE.md#reproducibility).

Other parts of the proof toolchain, including the K-framework, are licensed under different, open source terms, like those of The University of Illinois/NCSA Open Source License.

## Disclaimer

This repository does not constitute legal or investment advice. The preparers of this repository present it as an informational exercise documenting the due diligence involved in the secure development of the target contract only, and make no material claims or guarantees concerning the contract's operation post-deployment. The preparers of this repository assume no liability for any and all potential consequences of the deployment or use of this contract.

*The formal verification results presented here only show that the target contract behaviors meet the formal (functional) specifications. Moreover, the correctness of the generated formal proofs assumes the correctness of the specifications and their refinement, the correctness of [KEVM], the correctness of the [K-framework]'s [reachability logic theorem prover], and the correctness of the [Z3] SMT solver. The presented result makes no guarantee about properties not specified in the formal specification. Importantly, the presented formal specification considers only the behaviors within the EVM, without considering the block/transaction level properties or off-chain behaviors, meaning that the verification result does not completely rule out the possibility of the contract being vulnerable to existing and/or unknown attacks.*

Smart contracts are still a nascent software arena, and their deployment and public offering carries substantial risk. This repository makes no claims that its analysis is fully comprehensive, and recommends always seeking multiple opinions and audits.

This repository is also not comprehensive in scope, excluding a number of components critical to the correct operation of this system.

The possibility of human error in the manual review process is very real, and we recommend seeking multiple independent opinions on any claims which impact a large quantity of funds.


[KEVM]: <https://github.com/kframework/evm-semantics>
[K-framework]: <http://www.kframework.org>
[reachability logic theorem prover]: <http://fsl.cs.illinois.edu/index.php/Semantics-Based_Program_Verifiers_for_All_Languages>
[K reachability logic prover]: <http://fsl.cs.illinois.edu/index.php/Semantics-Based_Program_Verifiers_for_All_Languages>
[Download]: <https://github.com/kframework/k5/releases>
[install]: <https://github.com/kframework/k5/blob/master/README.md>
[K tutorial]: <https://github.com/kframework/k5/tree/master/k-distribution/tutorial>
[K editor support]: <https://github.com/kframework/k-editor-support>
[Jellopaper]: <https://jellopaper.org/>
[KEVM technical report]: <https://www.ideals.illinois.edu/handle/2142/97207>
[KEVM research paper]: <http://fsl.cs.illinois.edu/FSL/papers/2018/hildenbrandt-saxena-zhu-rodrigues-daian-guth-moore-zhang-park-rosu-2018-csf/hildenbrandt-saxena-zhu-rodrigues-daian-guth-moore-zhang-park-rosu-2018-csf-public.pdf>
[Z3]: <https://github.com/Z3Prover/z3>
[eDSL]: </resources/edsl.md>
[ERC20]: <https://github.com/ethereum/EIPs/blob/master/EIPS/eip-20.md>
[ERC20-K]: <https://github.com/runtimeverification/erc20-semantics>
[ERC20-EVM]: </resources/erc20-evm.md>
[ERC777]: <https://github.com/ethereum/eips/issues/777>

[IELE]: <https://github.com/runtimeverification/iele-semantics>
[Solidity]: <https://solidity.readthedocs.io/en/develop/>
[Vyper]: <https://github.com/ethereum/vyper>
[reachability logic]: <http://fsl.cs.illinois.edu/index.php/Reachability_Logic>
[ERC777-K]: <https://github.com/runtimeverification/erc777-semantics>
