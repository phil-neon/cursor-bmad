# BMad Method v6 Alpha Installation Guide

## ⚠️ PowerShell Execution Policy Fix (If Needed)

If you get an error like "cannot be loaded. The file is not digitally signed", run this first:

```powershell
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope Process -Force
```

This sets the execution policy for the current PowerShell session only (safe and temporary).

## Quick Install Command

Run this command in your terminal from the project root:

```powershell
npx --yes bmad-method@alpha install
```

## Installation Steps

1. **Run the install command** (see above)

2. **When prompted for installation directory:**
   - Press `Enter` to accept the default (current project directory)
   - Or type the full path if you want a different location

3. **When asked "Install to this directory?":**
   - Type `Y` and press `Enter`

4. **Select modules to install:**
   - **BMM** (BMad Method Module) - **REQUIRED** for core development
   - **BMB** (BMad Builder Module) - **RECOMMENDED** for agent building
   - Use arrow keys to navigate, spacebar to select, Enter to confirm

## Verification

After installation completes, verify by checking:

```powershell
# Check if .bmad directory was created
ls .bmad

# Check if agents were installed
ls .bmad/bmm/agents/
```

You should see files like:
- `analyst.md`
- `architect.md`
- `dev.md`
- `pm.md`
- `sm.md`
- `tea.md`
- `ux-designer.md`
- `quick-flow-solo-dev.md`
- `tech-writer.md`

## Next Steps

After installation, initialize your first workflow in Cursor by invoking:
```
*workflow-init
```

The Analyst agent will guide you through the setup.

## Important Notes (v6 Alpha.22)

- Default output folder is now `_bmad-output` (not `docs`)
- Planning artifacts go to `_bmad-output/planning-artifacts`
- Implementation artifacts go to `_bmad-output/implementation-artifacts`
- Long-term docs go to `docs/`

## Troubleshooting

### PowerShell Execution Policy Error
If you see "cannot be loaded. The file is not digitally signed":
```powershell
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope Process -Force
```
Then retry the installation command.

### Other Issues
- Check the [BMAD-METHOD GitHub repository](https://github.com/bmad-code-org/BMAD-METHOD)
- Ensure Node.js 20+ and npm 9+ are installed
- Make sure you're in the correct project directory
- If the execution policy keeps resetting, you may need to run PowerShell as Administrator and set it for CurrentUser:
  ```powershell
  Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
  ```
