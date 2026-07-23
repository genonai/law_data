# law_data

현행 시행 **법령류**(법률·시행령·시행규칙) 미러 저장소.

- **자동 생성**입니다. 손으로 편집하지 마세요. `temporal_law` 파이프라인(`pipeline/gitexport.py`)이 수집할 때마다 이 레포에 커밋·push 합니다.
- 각 법령의 본문을 **인라인 링크·이미지가 박힌 Markdown** 으로 미러링합니다. (위임·인용·조례·정관 링크, 별표/별지/서식, ⏳시행예정·⛔폐지예정 표시 포함)
- **현행(nw3) + 시행예정(nw2)** 버전을 병합해 담고, 폐지된 법령은 주기적으로 `git rm` 됩니다.
- 원본 데이터·메타데이터는 Postgres `lawdb` 에도 함께 적재됩니다. 이 레포는 사람이 읽기 좋은 미러입니다.

> 생성 주체: [temporal_law](https://github.com/sehunpark-genon/temporal_law) · `LAW_ENABLED=true`
