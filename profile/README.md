# Electron Publish Pro

> Managed build infrastructure for Electron apps. Code signing, notarization, and store publishing — without CI/CD complexity.

**Think Expo, but for Electron.**

## 🚀 What We Do

We take the pain out of publishing Electron applications:

- 🔄 **Sync** code from GitHub to our secure cloud
- 🔨 **Build** for macOS, Windows, and Linux in parallel
- ✍️ **Sign** with Apple Developer & Windows Authenticode certificates
- 🍎 **Notarize** automatically for macOS
- 📦 **Publish** to Mac App Store, Microsoft Store, Snap Store, or GitHub Releases

## 📦 Our Packages

| Package | Description | Status |
|---------|-------------|--------|
| [`@electron-publish-pro/sdk`](https://github.com/electron-publish-pro/sdk) | JavaScript/TypeScript SDK | 🚧 Soon |
| [`@electron-publish-pro/cli`](https://github.com/electron-publish-pro/cli) | Command-line interface | 🚧 Soon |
| [`docs`](https://github.com/electron-publish-pro/docs) | Documentation | 🚧 Soon |

## ⚡ Quick Example

```typescript
import { ElectronPublishPro } from '@electron-publish-pro/sdk';

const client = new ElectronPublishPro({ apiKey: 'your-api-key' });

// Trigger a build for all platforms
const build = await client.builds.create({
  projectId: 'my-project',
  platforms: ['macos', 'windows', 'linux'],
  version: '1.0.0'
});

// Check build status
const status = await client.builds.get(build.id);
console.log(status); // { status: 'completed', artifacts: [...] }
```

## 🔗 Links

- 🌐 [Website](https://electronpublish.com)
- 📖 [Documentation](https://electronpublish.com/docs)
- 🔒 [Security](https://electronpublish.com/security)
- 🐦 [Twitter](https://twitter.com/aspect_pub)

## 📊 Status

🚧 **Coming Soon** — [Join the waitlist](https://electronpublish.com)

---

**Built with ❤️ for Electron developers**
