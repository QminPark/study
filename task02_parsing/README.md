### 먼저 다음 명령어를 실행시켜서 예제 데이터를 다운 받도록 하자.
```
wget https://raw.githubusercontent.com/JunKimCNU/JunKimLabTutorial/main/task02_parsing/cb4856.substr.fa
wget https://raw.githubusercontent.com/JunKimCNU/JunKimLabTutorial/main/task02_parsing/lsp41_scaffolds.substr.fa
```
### 그 뒤 다음 질문에 대해 답해보자.
```
(1) (grep and/or wc 등을 활용) lsp41_scaffolds.substr.fa 에 포함된 시퀀스 개수는?(힌트: 모든 시퀀스의 이름은 > 로 시작함) (힌트: 파이프를 활용해서 여러 명령어를 연달아 적용해보자.)
(2) (grep and/or wc 등을 활용) cb4856.substr.fa 파일에 포함된 시퀀스 개수는?
(3) (sed 활용) cb4856.substr.fa 에 포함된 시퀀스 이름은 "tig00015902|quiver|quiver|pilon|pilon" 등으로 되어있다. 여기서 |quiver|quiver|pilon|pilon 부분을 제거하고 싶다면 어떻게 해야 할까?
(4) (grep and/or wc 등을 활용) Assemblytics_structural_variants.bed 는 50 bp 이상의 structural variants에 관한 정보를 포함하는 tab으로 분리된 형식이다(tab-separated values; tsv). 2번 염색체에는 몇 개의 variant가 존재하는가? (힌트: grep -P "\t" or grep -w or grep "<>")
(5) (grep and/or wc 등을 활용) 2번 염색체에 생긴 variant 중 insertion은 몇 개인가? (힌트: 7번째 컬럼 정보를 확인해보기)
(6) (sort 및 head 활용) 이 중 가장 크기가 큰 구조 변이 15개에 대한 정보만 포함하는 파일을 만들어 보자.
(첫 번째 힌트: sort는 기본적으로는 사전순으로 정렬하기 때문에, 567과 58이 있을 때 58이 더 크다고 판단함. 이런 걸 보완하는 옵션을 알아보자.
두 번째 힌트: sort를 활용하면 몇 번째 컬럼을 기준으로 정렬할지도 정할 수 있으니 그 옵션을 활용해보자.)
```
