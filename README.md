# SushiSwap Agent Skills

Agent Skills for integrating the **SushiSwap Swap Aggregator** into your applications.  
These skills teach AI agents how to help developers implement optimized token swaps,
pricing, and executable transaction generation using the
[SushiSwap SDK](https://github.com/sushi-labs/sushi) and
[SushiSwap REST API](https://api.sushi.com).

---

## Installation

Install all skills from this repository:

```bash
npx skills add sushi-labs/agent-skills
```

Or install individual skills:

```bash
npx skills add sushi-labs/agent-skills/sushiswap-sdk
npx skills add sushi-labs/agent-skills/sushiswap-api
```

---

## Available Skills

### sushiswap-sdk

TypeScript SDK integration for the SushiSwap Aggregator.  
Covers requesting swap quotes, generating executable swap transactions, working
with strongly typed token and amount primitives, and safely simulating or
executing swaps.

Use when:
- Building TypeScript or JavaScript applications
- You want to use strongly typed token, amount, and price primitives available in the sushi package
- You prefer SDK-based integration over raw HTTP

---

### sushiswap-api

Direct integration with the SushiSwap REST API.  
Covers swap quoting, swap transaction generation, token pricing, token metadata,
and discovery of supported liquidity sources.

Use when:
- Building backend services or bots
- Working in non-JavaScript environments
- You need direct HTTP access to the SushiSwap Aggregator
- You want full control over request construction and execution

---

## What is SushiSwap?

[SushiSwap](https://www.sushi.com) is a multichain decentralized exchange and
swap aggregation protocol focused on best execution.

It provides:
- DEX aggregation across many AMMs
- Optimized routing for best price selection
- Executable transaction calldata generation with optional on-chain simulation

The SushiSwap Aggregator powers both the SDK and REST API integrations
described in these skills.

---

## Supported Networks

The SushiSwap Aggregator supports 40+ EVM-compatible chains.

Supported networks can be discovered dynamically via:
- SDK helpers such as SWAP_API_SUPPORTED_CHAIN_IDS

Agents must not assume hardcoded network support.

---

## Resources

- Documentation: https://docs.sushi.com
- API Base URL: https://api.sushi.com
- GitHub: https://github.com/sushi-labs
- SDK Source: https://github.com/sushi-labs/sushi