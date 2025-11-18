# 🔍 VaultPlay Draw Verifier

Independent verification tool that allows competition participants to reconstruct and verify their draw results step-by-step using publicly available audit data.

## 🎯 What Does This Tool Do?

This tool helps you verify that your competition entry was processed fairly by:

1. **Finding Your Draw** - Locates your entry in our public audit repository
2. **Verifying Randomness** - Checks the public randomness source (drand)
3. **Showing Seed Generation** - Demonstrates how the draw seed was created
4. **Calculating Your Score** - Shows exactly how your unique score was computed
5. **Displaying Your Rank** - Reveals where you placed among all entries

## 🚀 Live Demo

**Try it now:** [https://vaultplay-dev.github.io/vaultplay-draw-verifier/](https://vaultplay-dev.github.io/vaultplay-draw-verifier/)

## 💡 Why Open Source?

We believe in **radical transparency**. By making this verification tool open source:

- ✅ Anyone can inspect the verification logic
- ✅ Security researchers can audit the code
- ✅ You can verify draws without trusting us
- ✅ The community can contribute improvements

## 🔒 How It Works

### The VaultPlay Draw System

Every VaultPlay draw uses:
- **Public randomness** from [drand.love](https://drand.love) (distributed randomness beacon)
- **SHA-256 hashing** for deterministic scoring
- **Public audit bundles** stored on GitHub for verification

### Verification Process
```
Your Entry Code
    ↓
Search Audit Bundles → Find Your Draw
    ↓
Fetch drand Randomness → Verify Public Source
    ↓
Generate Seed (SHA-256) → Hash Randomness
    ↓
Calculate Score (SHA-256) → Hash (Seed + Your Code)
    ↓
Compare Scores → Rank All Entries
    ↓
Your Final Position ✓
```

## 🛠️ Technical Stack

- **Pure HTML/CSS/JavaScript** - No frameworks, no build process
- **Web Crypto API** - SHA-256 hashing in the browser
- **GitHub API** - Fetches public audit bundles
- **drand API** - Verifies randomness sources
- **GitHub Pages** - Free, fast, and secure hosting

## 📚 Related Repositories

- **Draw Worker:** [vaultplay-draw-worker](https://github.com/vaultplay-dev/vaultplay-draw-worker) - The system that executes draws
- **Audit Repository:** [vaultplay-draw-history](https://github.com/vaultplay-dev/vaultplay-draw-history) - Public audit trail of all draws

## 🤝 Contributing

We welcome contributions! If you find a bug or want to improve the tool:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/improvement`)
3. Commit your changes (`git commit -am 'Add improvement'`)
4. Push to the branch (`git push origin feature/improvement`)
5. Open a Pull Request

## 📖 Documentation

For more information about how VaultPlay draws work:
- **How Draws Work:** https://vaultplay.co.uk/how-draws-work
- **Draw Worker Documentation:** https://github.com/vaultplay-dev/vaultplay-draw-worker

## 📄 License

MIT License - see [LICENSE](LICENSE) for details

## 🔗 Links

- **Website:** [vaultplay.co.uk](https://vaultplay.co.uk)
- **Verification Tool:** [verify.vaultplay.co.uk](https://verify.vaultplay.co.uk) *(or GitHub Pages URL)*
- **Contact:** [Contact page](https://vaultplay.co.uk/contact)

---

**Built with transparency in mind** | Made by [VaultPlay](https://vaultplay.co.uk)
```

---
