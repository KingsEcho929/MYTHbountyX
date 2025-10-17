🛡️ Hybra Finance Audit Report — MYTHbountyX
Auditor: Chase Todd Hawkins (.CTH) Platform: Code4rena Date: October 15, 2025 Repo: hybra-audit/2025-10-hybra-finance Scope: ve33/contracts, CLGauge, Governance, Bribes, Mocks, Libraries, Tests

🔐 High Severity Findings
ID	File	Title	Impact
H-01	VoterV3.sol	Bribe Withdrawal Reentrancy	Reentrancy via external bribe contracts
H-02	GaugeCL.sol	Reentrancy Risk in getReward	Unprotected reward transfer logic
H-03	HYBR.sol	Unsealed mint() Function	Arbitrary token minting
H-04	GovernanceHYBR.sol	Timelock Bypass Risk	Immediate proposal execution
H-05	VotingEscrow.sol	Griefable create_lock() via Timestamps	State bloat and vote weight distortion
H-06	RewardHYBR.sol	Reentrancy Risk in getReward	Unprotected reward logic
H-07	Bribes.sol	Reentrancy Risk in getReward	Unprotected bribe logic
H-08	MinterUpgradeable.sol	Unsealed mint() Function	Arbitrary token minting
H-09	GaugeFactoryCL.sol	Unsealed setGaugeLogic()	Logic hijack risk
⚠️ Medium Severity Findings
ID	File	Title	Impact
M-01	GaugeManager.sol	Missing Access Control	Unauthorized gauge creation
M-02	Bribes.sol	Unsafe ERC20 Assumptions	Griefable token transfers
M-03	GaugeCL.sol	Precision Loss in earned()	Reward miscalculation
M-04	VotingEscrow.sol	Griefable merge() Logic	Vote hijack or grief
M-05	GovernanceHYBR.sol	Proposal Griefing via Unrestricted Access	Governance spam
M-06	VotingEscrow.sol	Missing Ownership Check in merge()	Unauthorized merge
M-07	RewardHYBR.sol	Missing Input Validation in notifyRewardAmount()	Gas grief or reward spam
M-08	Bribes.sol	Unsafe deposit() Logic	Griefable token transfers
M-09	MinterUpgradeable.sol	Missing Input Validation in notifyRewardAmount()	Reward spam
M-10	HYBR.sol	Replay Risk in permit()	Signature reuse
M-11	VotingBalanceLogic.sol	Rounding Loss in calculateVotingPower()	Vote weight distortion
M-12	GaugeFactoryCL.sol	Griefable createGauge()	Registry bloat
🧪 Low Severity Findings
ID	File	Title	Impact
L-01	GaugeCL.sol	Missing Input Validation	Gas grief or edge-case spam
L-02	VeArtProxyUpgradeable.sol	Missing Access Control in setBaseURI()	Metadata hijack
L-03	GovernanceHYBR.sol	Missing Input Validation in castVote()	Zero-weight votes
L-04	VotingEscrow.sol	Missing Input Validation in increase_amount()	Gas grief
L-05	Bribes.sol	Missing Input Validation in notifyRewardAmount()	Bribe spam
L-06	HYBR.sol	Missing initializer Modifier	Upgrade risk
L-07	VotingBalanceLogic.sol	Missing Delegation Sync	Stale vote weight
