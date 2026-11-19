# SupoClip customizations

This repository currently stores the patch for the SupoClip installation prepared in ChatGPT. It is based on upstream commit `c4512645e48b7d961766239b5574b62c71b3a1ae` and improves spoken hooks and clip endings.

To create a working copy on your computer:

```bash
git clone https://github.com/FujiwaraChoki/supoclip.git
cd supoclip
git checkout c4512645e48b7d961766239b5574b62c71b3a1ae
curl -L https://raw.githubusercontent.com/Jomarte/supoclips/main/supoclip-hook-endings.patch -o supoclip-hook-endings.patch
git am supoclip-hook-endings.patch
```

Keep API keys in ignored `.env` files. The patch contains no credentials or video files.
