# ForgePress path-based GitHub Pages starter

## Folder layout
- `index.html` → `/buktijepe/`
- `login/index.html` → `/buktijepe/login/`
- `admin/index.html` → `/buktijepe/admin/`
- `admin/posts/index.html` → `/buktijepe/admin/posts/`
- `admin/settings/index.html` → `/buktijepe/admin/settings/`
- `admin/pages/index.html` → `/buktijepe/admin/pages/`
- `admin/media/index.html` → `/buktijepe/admin/media/`

GitHub Pages serves directory `index.html` files directly. The browser may normalize a directory URL by adding a trailing slash. Both slash/no-slash links should resolve.

## Deploy
Upload the CONTENTS of this folder into the root of repository `buktijepe` (not the folder itself), preserving the directory structure. Keep GitHub Pages configured to `main` and `/(root)`.

## Important
- `BASE_PATH` is set to `/buktijepe` because this is a GitHub project site.
- Login is only a frontend shell until `GAS_API_URL` is configured and the GAS backend is implemented.
- Do not rely on client-side route hiding as security. GAS must validate expiring session tokens on every protected read/write request.
- Keep private content out of the public GitHub repository.
