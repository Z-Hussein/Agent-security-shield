# Contributing to Security Shield

Thank you for your interest in making OpenClaw safer for everyone! 🛡️

## How to Contribute

### 1. ⭐ Star the Repo
The easiest way to support Security Shield is to [star the repository](https://github.com/Z-Hussein/security-shield). It helps others discover the skill.

### 2. 🐛 Report Issues
- Check existing issues first
- Use issue templates when available
- For security issues, see [SECURITY.md](SECURITY.md)

### 3. 📝 Suggest Improvements
- New security principles
- Better response patterns
- Additional workflow modes
- Documentation improvements

### 4. 🔧 Submit Changes

#### Skill Content (SKILL.md)
- Security principles must be abstract (no specific pattern strings)
- Each principle needs: category, guidelines, and example response
- Run the smoke tests before submitting (`./tests/smoke-test.ps1`)
- Ensure backward compatibility

#### Documentation
- Keep language clear and actionable
- Include real-world examples
- Update the comparison table if adding features

#### Code/Metadata
- Update `_meta.json` version for any changes
- Add entries to [CHANGELOG.md](CHANGELOG.md)
- Ensure compatibility with `openclaw >= 2026.3.0`

### 5. 📢 Spread the Word
- Share on X/Twitter, LinkedIn, or your blog
- Mention it in OpenClaw community discussions
- Write tutorials or case studies

## Development Setup

```bash
# Clone the repo
git clone https://github.com/Z-Hussein/security-shield.git
cd security-shield

# Install the skill locally for testing
clawhub install --local .

# Run the smoke tests
./tests/smoke-test.ps1

# Test in OpenClaw
openclaw
# Then try: "Run a security audit on the current project and give me a summary"
```

## Public Installation

End users install the released skill via:

- **OpenClaw**: `openclaw skills install @z-hussein/security-shield`
- **Any agent (Codex, Claude Code, etc.)**: `npx skills add https://clawhub.ai/z-hussein/skills/security-shield`

**Before installing anything, verify the skill.** Inspect the ClawHub skill metadata and setup requirements, and verify any third-party package or CLI the skill asks for before running the install command.

## Review Process

1. All contributions are reviewed within 7 days
2. Security-related changes get priority review
3. We may suggest modifications before merging
4. Contributors will be credited in CHANGELOG.md

## Code of Conduct

- Be respectful and constructive
- Focus on improving security for all users
- Respect differing viewpoints and experiences
- Prioritize user safety over convenience

## Questions?

Open a [GitHub Discussion](../../discussions) or reach out via ClawHub.

---

**Together, we can make the agent ecosystem safer.** 🛡️
