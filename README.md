# Password Generator

A feature-rich desktop password generator application built with Python and Tkinter. Supports both random password generation and passphrase creation with real-time strength analysis.

## Features

**Dual Generation Modes**
- **Random Password Mode**: Customizable length (6-32 characters) with toggleable character sets
- **Passphrase Mode**: Cryptographically-secure multi-word passphrases (3-8 words)

**Security**
- Uses `secrets` module for cryptographically strong random generation
- Real-time password strength analysis with visual feedback
- Support for uppercase, lowercase, numbers, and special characters

**User Interface**
- Clean, intuitive Tkinter GUI with responsive design
- Live strength indicator with color-coded feedback (Weak/Medium/Strong)
- One-click copy to clipboard functionality
- Radio button mode switching for seamless UX

**Strength Analysis Algorithm**
- Multi-factor evaluation based on:
  - Length thresholds (8+ and 14+ characters)
  - Character variety (uppercase, lowercase, digits, symbols)
- Three-tier scoring system with visual strength bar

## Installation

### Requirements
- Python 3.7+
- Tkinter

### Setup
```bash
git clone https://github.com/user/password-generator.git
cd password-generator
python password_generator.py
```

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

## Future Enhancements

- [ ] Google Chrome extension capability
- [ ] Custom word list import for passphrases
- [ ] Dark mode theme
- [ ] Keyboard shortcuts (Enter to generate, Ctrl+C to copy)
- [ ] Password history with deletion

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
