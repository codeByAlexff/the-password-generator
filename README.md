# Password Generator

A feature-rich desktop password generator application built with Python and Tkinter. Supports both random password generation and passphrase creation with real-time strength analysis.

## Features

✨ **Dual Generation Modes**
- **Random Password Mode**: Customizable length (6-32 characters) with toggleable character sets
- **Passphrase Mode**: Cryptographically-secure multi-word passphrases (3-8 words)

🔒 **Security**
- Uses `secrets` module for cryptographically strong random generation
- Real-time password strength analysis with visual feedback
- Support for uppercase, lowercase, numbers, and special characters

🎨 **User Interface**
- Clean, intuitive Tkinter GUI with responsive design
- Live strength indicator with color-coded feedback (Weak/Medium/Strong)
- One-click copy to clipboard functionality
- Radio button mode switching for seamless UX

📊 **Strength Analysis Algorithm**
- Multi-factor evaluation based on:
  - Length thresholds (8+ and 14+ characters)
  - Character variety (uppercase, lowercase, digits, symbols)
- Three-tier scoring system with visual strength bar

## Installation

### Requirements
- Python 3.7+
- Tkinter (usually included with Python)

### Setup
```bash
git clone https://github.com/yourusername/password-generator.git
cd password-generator
python password_generator.py
```

## Usage

1. **Launch the application**
   ```bash
   python password_generator.py
   ```

2. **Choose your mode**
   - Select "Random password" or "Passphrase" via radio buttons

3. **Configure settings**
   - Adjust length/word count with the slider
   - Toggle character types (uppercase, lowercase, numbers, symbols)

4. **Generate & Copy**
   - Click "Generate" to create a new password
   - Click "Copy" to add to clipboard
   - Strength indicator updates automatically

## Technical Highlights

### Code Quality
- **Modular design**: Separate functions for password generation, passphrase creation, and strength analysis
- **Object-oriented**: App class encapsulates UI and logic
- **Security best practices**: Uses `secrets` module instead of `random`

### Key Functions
- `generate_password()`: Creates random passwords with configurable character sets
- `generate_passphrase()`: Selects cryptographically-secure word combinations from 50+ word list
- `analyze_strength()`: Evaluates password robustness using multi-factor scoring
- `update_ui()`: Dynamically manages UI visibility based on mode selection

### Design Patterns
- **State Management**: StringVar and BooleanVar for tracking UI state
- **Responsive Layout**: Pack geometry manager for flexible, adaptive design
- **Real-time Feedback**: Strength indicator updates on every generation

## Security Considerations

- ✅ Uses `secrets.choice()` for cryptographically-secure randomness
- ✅ Special characters limited to unambiguous symbols: `!@#$%^&*-`
- ✅ No external dependencies—no third-party vulnerability risks
- ✅ Clipboard operations use native Tkinter functionality

## Future Enhancements

- [ ] Password history with deletion
- [ ] Exclude ambiguous characters option (O/0, l/1, etc.)
- [ ] Custom word list import for passphrases
- [ ] Dark mode theme
- [ ] Keyboard shortcuts (Enter to generate, Ctrl+C to copy)
- [ ] Export to file functionality

## Project Structure

```
password-generator/
├── password_generator.py    # Main application file
└── README.md               # Documentation
```

## License

This project is open source and available under the MIT License.

## Author

Created as a demonstration of Python GUI development, security best practices, and user experience design.

---

**Why this project matters:**
This password generator demonstrates proficiency in Python desktop application development, security-conscious programming, and creating intuitive user interfaces. It showcases an understanding of cryptographic best practices while maintaining code clarity and maintainability.
