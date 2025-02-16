## git convention
모든 개발은 develop branch를 중심으로 진행합니다.

1. ISSUE 생성
2. 해당 branch 작업
3. PR 생성 후 confirm
4. merge to develop branch

## git commit message convention
| label | emoji | description |
|-------|-------|------------|
| devops | 🚚 | DevOps related changes |
| docs | 📝 | Documentation only changes |
| feat | ✨ | A new feature |
| refactor | 🔨 | A code change that neither fixes a bug nor adds a feature |
| setting | 🔧 | Changes to settings |
| test | ✅ | Adding missing tests or correcting existing tests |
| bug | 🐛 | A bug fix |
| question | 💡 | A question |

## branch 자동 생성
issue 생성 시 branch가 자동 생성됩니다.
- devops, docs, feat, refactor, setting, test 라벨이 붙은 issue는 feature/ 브랜치로 생성됩니다.
- bug 라벨이 붙은 issue는 hotfix/ 브랜치로 생성됩니다.
- question 라벨이 붙은 issue는 따로 브랜치가 생성되지 않습니다.
```
{label}/{issue-number}-{domain}
ex) feature/#25-rent
```

💡 ISSUE나 PR에 이모지와 함께 사용하면 더욱 보기 좋습니다.

## PR label 자동 설정
PR title에 위 표에 나와있는 label name 혹은 emoji를 포함하면 자동으로 label이 설정됩니다.

💡 직접 설정하셔도 됩니다.
