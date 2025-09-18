# SYJ-MINI Token Presale Website

Next.js 14 website for the SYJ-MINI token presale. Built with TypeScript, TailwindCSS, and Web3Modal.

## Quick Start

1. Install dependencies:
```bash
pnpm install
```

2. Configure environment:
```bash
cp .env.local.example .env.local
# Fill in your values
```

3. Run development server:
```bash
pnpm dev
```

## Configuration

### Environment Variables

- `NEXT_PUBLIC_WALLETCONNECT_PROJECT_ID`: Your WalletConnect project ID
- `NEXT_PUBLIC_RPC_HTTP`: Ethereum RPC URL (Alchemy/Infura)
- `NEXT_PUBLIC_PRESALE_ADDRESS`: Presale contract address
- `NEXT_PUBLIC_SYJMINI_ADDRESS`: Token contract address
- `NEXT_PUBLIC_CHAIN_ID`: 1 for mainnet, 11155111 for Sepolia testnet

### Switch to Testnet

1. Set `NEXT_PUBLIC_CHAIN_ID=11155111` in `.env.local`
2. Update `NEXT_PUBLIC_RPC_HTTP` to your Sepolia RPC URL
3. Deploy contracts to Sepolia and update addresses

## Development

- `pnpm dev` - Start development server
- `pnpm build` - Build for production
- `pnpm start` - Start production server
- `pnpm lint` - Run linting

## Features

- Next.js 14 App Router
- TypeScript & TailwindCSS
- Web3Modal v3 integration
- Presale widget & calculator
- Responsive design
- SEO optimized
- Analytics ready

## Deployment

### Vercel (Recommended)
1. Import repository
2. Configure environment variables
3. Deploy

### Static Export
1. Update `next.config.js` with `output: 'export'`
2. Run `pnpm build`
3. Deploy `out` directory

## Contract Integration

1. Update contract addresses in `.env.local`
2. Verify contract ABIs match `lib/abi/`
3. Test transactions on Sepolia first
4. Update presale parameters in `lib/constants.ts`

## License

MIT

