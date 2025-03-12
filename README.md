### Installation

Requirements: `tmux` version 1.9 (or higher), `git`, `bash`.

Clone TPM:

```bash
git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm
```

### Prefix Key:
I’ve remapped the prefix key from `Ctrl+b` to `Ctrl+Space`:

- **Prefix Key**: `Ctrl+Space`

To perform any Tmux command, you need to press `Ctrl+Space`, then the desired command key.

---

### Key Bindings in Your Setup

#### **Window and Pane Navigation:**

- **Create a new window**: 
  - `Ctrl+Space` followed by `c`
  
- **Switch to next window**:
  - `Ctrl+Space` followed by `n`
  
- **Switch to previous window**:
  - `Ctrl+Space` followed by `p`

- **Switch to a specific window by number**:
  - `Ctrl+Space` followed by `1`, `2`, `3`, etc. (for window numbers)

- **Rename the current window**:
  - `Ctrl+Space` followed by `,`

- **Close the current window**:
  - `Ctrl+Space` followed by `&`

---

#### **Pane Navigation (Vim-style)**

I’ve configured Vim-style keybindings for selecting panes:

- **Move to the left pane**:
  - `Ctrl+Space` followed by `h` (move left)

- **Move to the down pane**:
  - `Ctrl+Space` followed by `j` (move down)

- **Move to the up pane**:
  - `Ctrl+Space` followed by `k` (move up)

- **Move to the right pane**:
  - `Ctrl+Space` followed by `l` (move right)

---

#### **Mouse Support**:
- **Mouse mode is enabled**: You can click on panes to switch between them, resize panes with the mouse, and scroll through the terminal content.

---

#### **Pane Splitting**:

- **Split the window vertically** (left-right):
  - `Ctrl+Space` followed by `v`

- **Split the window horizontally** (top-bottom):
  - `Ctrl+Space` followed by `b`

---

#### **Additional Keybindings for Switching Panes (Using Alt + Arrow Keys)**

I've configured the following to switch panes directly without the prefix key (`Ctrl+Space`):

- **Move to the left pane**:
  - `Alt+Left Arrow` (no prefix)

- **Move to the right pane**:
  - `Alt+Right Arrow` (no prefix)

- **Move to the up pane**:
  - `Alt+Up Arrow` (no prefix)

- **Move to the down pane**:
  - `Alt+Down Arrow` (no prefix)

---

#### **Window Switching (Shift + Arrow)**

I’ve also set up these keybindings for switching between windows without the prefix:

- **Switch to the previous window**:
  - `Shift+Left Arrow` (no prefix)

- **Switch to the next window**:
  - `Shift+Right Arrow` (no prefix)

---

#### **Window Switching (Alt + H and Alt + L)**

You can switch windows using the `Alt` key with `H` and `L`:

- **Switch to the previous window**:
  - `Alt+H` (no prefix)

- **Switch to the next window**:
  - `Alt+L` (no prefix)

---

#### **Copy Mode (Vim-style)**

I’ve enabled Vim-style keybindings in copy mode:

- **Enter copy mode**:
  - `Ctrl+Space` followed by `[` (enter copy mode)

- **Start selecting text in copy mode**:
  - Press `v` (Vim-style) in copy mode
  
- **Copy selected text**:
  - `Ctrl+Space` followed by `y`

- **Cancel copy mode and exit**:
  - `q` (while in copy mode)

- **Toggle rectangle selection**:
  - `Ctrl+Space` followed by `C-v` in copy mode

---

#### **Other Custom Settings**:

- **Start windows and panes at 1 instead of 0**:
  - I’ve set this with:
    ```bash
    set -g base-index 1
    set -g pane-base-index 1
    set-window-option -g pane-base-index 1
    set-option -g renumber-windows on
    ```

- **Enable Vi-mode for copy mode**:
  - This enables Vim-style navigation in copy mode:
    ```bash
    set-window-option -g mode-keys vi
    ```

- **Set your terminal's flavour to Catppuccin Mocha** (for the Catppuccin theme):
  - `set -g @catppuccin_flavour 'mocha'`

- **Tmux Plugins**:
  - I have several Tmux plugins configured, such as `tmux-plugins/tpm`, `tmux-sensible`, `vim-tmux-navigator`, and others. You can install them using the `prefix + I` keybinding (with `Ctrl+Space` as the prefix).

---

### All Keybindings:

- **Prefix Key**: `Ctrl+Space`
- **Create Window**: `Ctrl+Space` followed by `c`
- **Switch to Next Window**: `Ctrl+Space` followed by `n`
- **Switch to Previous Window**: `Ctrl+Space` followed by `p`
- **Switch Window by Number**: `Ctrl+Space` followed by `1, 2, 3...`
- **Rename Window**: `Ctrl+Space` followed by `,`
- **Close Window**: `Ctrl+Space` followed by `&`
- **Split Vertically**: `Ctrl+Space` followed by `%`
- **Split Horizontally**: `Ctrl+Space` followed by `"`
- **Vim-style Pane Navigation**:
  - Left: `Ctrl+Space` followed by `h`
  - Down: `Ctrl+Space` followed by `j`
  - Up: `Ctrl+Space` followed by `k`
  - Right: `Ctrl+Space` followed by `l`
- **Alt Arrow Keys for Pane Switching** (no prefix):
  - Left: `Alt+Left Arrow`
  - Right: `Alt+Right Arrow`
  - Up: `Alt+Up Arrow`
  - Down: `Alt+Down Arrow`
- **Shift Arrow Keys for Window Switching** (no prefix):
  - Left: `Shift+Left Arrow`
  - Right: `Shift+Right Arrow`
- **Alt + H for Previous Window** (no prefix)
- **Alt + L for Next Window** (no prefix)
- **Enter Copy Mode**: `Ctrl+Space` followed by `[`
- **Start Selection in Copy Mode**: `v` (in copy mode)
- **Copy Selection**: `Ctrl+Space` followed by `y`
- **Cancel Copy Mode**: `q`
- **Toggle Rectangle Selection**: `Ctrl+Space` followed by `C-v`

---
