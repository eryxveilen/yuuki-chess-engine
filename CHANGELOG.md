# Changelog

All notable changes to Yuuki Chess Engine are documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.1.0] - 2026-06-27

### Added
- Cross-platform build system with CMake
- Multi-architecture support (x86_64, ARM64, Windows)
- GitHub Actions continuous integration
- Automated release build workflow
- Docker containerization support
- Comprehensive build documentation (BUILD.md)
- Release procedures guide (RELEASE.md)

### Features
- Full UCI (Universal Chess Interface) protocol support
- Advanced alpha-beta pruning with iterative deepening
- Principal Variation Search (PVS)
- Configurable transposition table (1–4096 MB)
- Sophisticated tapered evaluation with 25+ feature components
- Move optimizations: LMR, null-move pruning, futility pruning, razoring, aspiration windows
- Quiescence search with delta pruning and SEE
- Skill levels (0–20) for handicap play
- Polyglot-compatible opening book support
- Up to 512 configurable threads
- 50+ customizable evaluation parameters

### Evaluation Components
- Material and piece-square tables (tapered MG/EG)
- Piece mobility bonuses
- Pawn structure analysis (isolated, doubled, backward, passed, etc.)
- King safety (pawn shield, pawn storm, attack zones)
- Rook and minor piece evaluation
- Threat detection and trapped pieces
- Space control and tropism
- Pins and discovered attacks
- Material imbalance handling
- Initiative and tactical motifs

### Known Issues
- Web app PGN/FEN detection may be unreliable

### Credits
- **Developer**: Eryx/RJ
- **Inspired by**: Stockfish, Ethereal, and open-source chess community

## [1.0] - Initial Release

### Added
- Initial Yuuki Chess Engine release
- Complete UCI protocol implementation
- Full chess rule support (castling, en passant, promotion)
- Evaluation function with PST tables
- Search algorithms with transposition tables
- Zobrist hashing for position identification
- Move generation and validation
- Quiescence search
- Basic move ordering

---

## Version Tags

Releases are tagged as `v{MAJOR}.{MINOR}.{PATCH}` on GitHub.

To fetch a specific version:
```bash
git checkout v1.1.0
```

To download pre-built binaries, visit [Releases](https://github.com/eryxveilen/yuuki-chess-engine/releases).
