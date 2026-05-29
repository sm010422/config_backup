# dotfiles / config backup

macOS 개발 환경 설정 파일 백업 저장소입니다.

## 구조

```
config_backup/
├── atuin/          # 쉘 히스토리 관리 (atuin)
├── bashtop/        # 리소스 모니터 (bashtop)
├── broot/          # 파일 탐색기 (broot)
├── btop/           # 리소스 모니터 (btop)
├── configstore/    # CLI 도구 설정 저장소
├── fastfetch/      # 시스템 정보 출력 (fastfetch)
├── fish/           # Fish 쉘 설정
├── gh/             # GitHub CLI 설정
├── gh-dash/        # GitHub 대시보드 TUI (gh-dash)
├── ghostty/        # 터미널 에뮬레이터 설정 (Ghostty)
├── git/            # Git 글로벌 설정 (gitignore)
├── github-copilot/ # GitHub Copilot 설정
├── gitui/          # Git TUI 클라이언트 (gitui)
├── htop/           # 프로세스 모니터 (htop)
├── iterm2/         # 터미널 에뮬레이터 설정 (iTerm2)
├── kafkactl/       # Kafka CLI 설정
├── karabiner/      # 키보드 커스터마이징 (Karabiner-Elements)
├── lazydocker/     # Docker TUI 클라이언트 (lazydocker)
├── lnav/           # 로그 파일 뷰어 (lnav)
├── mc/             # 파일 관리자 (Midnight Commander)
├── neofetch/       # 시스템 정보 출력 (neofetch)
├── nvim/           # Neovim 설정 (LazyVim 기반)
├── pip/            # Python 패키지 매니저 설정
├── posting/        # HTTP 클라이언트 TUI (posting)
├── vercel-plugin/  # Vercel 플러그인 세션 정보
└── wtf/            # 터미널 대시보드 (wtf)
```

## 주요 도구

| 분류 | 도구 |
|------|------|
| **쉘** | Fish, Atuin |
| **에디터** | Neovim (LazyVim) |
| **터미널** | Ghostty (주), iTerm2 |
| **Git** | gh CLI, gh-dash, gitui |
| **모니터링** | btop, bashtop, htop, wtf |
| **파일 탐색** | broot, mc |
| **기타 TUI** | lazydocker, lnav, posting |
| **시스템 정보** | fastfetch, neofetch |
| **키보드** | Karabiner-Elements |
| **인프라** | kafkactl |

## 복원 방법

각 디렉토리의 파일을 `~/.config/<tool>/` 또는 해당 도구의 설정 경로로 복사합니다.

```bash
# 예시: fish 설정 복원
cp -r fish/ ~/.config/fish/

# 예시: nvim 설정 복원
cp -r nvim/ ~/.config/nvim/

# 예시: ghostty 설정 복원
cp -r ghostty/ ~/.config/ghostty/
```

### 주요 경로

| 도구 | 설정 경로 |
|------|-----------|
| fish | `~/.config/fish/` |
| nvim | `~/.config/nvim/` |
| ghostty | `~/.config/ghostty/` |
| atuin | `~/.config/atuin/` |
| btop | `~/.config/btop/` |
| broot | `~/.config/broot/` |
| gh | `~/.config/gh/` |
| gh-dash | `~/.config/gh-dash/` |
| karabiner | `~/.config/karabiner/` |
| lazydocker | `~/Library/Application Support/lazydocker/` |
| kafkactl | `~/.config/kafkactl/` |
| git (ignore) | `~/.config/git/ignore` |
