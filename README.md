# `git-jijin` :boom:

### ![Inspiration](https://github.com/todoaskit/git-jijin/blob/master/pic/git-jijin.jpg)

`git-jijin`은 `git-fire`에서 포크한 프로젝트로, `fire`이 `jijin`으로 바뀌고 일부 명령어가 한국어로 번역된 것을 제외하면 완전히 똑같습니다.

적용법:  
git-jijin을 `$PATH`에 실행가능한 상태 (`chmod +x git-fire`)로 두시면 됩니다. (`$PATH`를 확인하시려면 terminal에서 `echo $PATH`를 실행하세요.)

사용법:  
`git-jijin <message>`  
메시지는 옵션입니다. 입력되지 않으면 `"지진이다! Branch $(current_branch)."`가 자동으로 사용됩니다.

아래는 `git-fire`의 `readme.md`입니다.

________________


`git-fire` is a Git plugin that **helps in the event of an emergency** by switching to the repository's root directory, adding all current files, committing, and pushing commits and all stashes to a new branch (to prevent merge conflicts).

**Alias it to [`git out`](https://np.reddit.com/r/ProgrammerHumor/comments/3nc531/in_case_of_fire/cvmxnv1) or [`git going`](https://np.reddit.com/r/ProgrammerHumor/comments/3nc531/in_case_of_fire/cvmsajb) for comedic effect.**

- `git config --global alias.out fire`
- `git config --global alias.going fire`

## What It Does

- changes directory to root directory of the repository
- creates new branch `fire-<current branch>-<user email>-<current epoch>`
- adds all files
- commits with `"Fire! Branch <new branch>"` or custom message
- pushes commits to remote
- pushes all stashes to remote

## Usage

`git-fire <message>`

`<message>` is optional. If not specified, `"Fire! Branch fire-<current branch>-<user email>-<current epoch>"` will be used.

## Installation

Just copy `git-fire` to your `$PATH` and ensure it is an executable (`chmod +x git-fire`) and you're good to go. 👍

`git-fire` is also available via [`npm`](https://npmjs.com/git-fire). Just run `npm install -g git-fire`, which will copy the `git-fire` binary to your `$PATH`.

Also make sure you have Git installed.

## Disclaimer

Your life is always more valuable than any code. You should leave the building immediately in a true emergency.

Code can be re-written, but humans cannot.

## Credit

Originally seen on [Hackathon Hackers Facebook](https://www.facebook.com/groups/hackathonhackers) group.

[Original Reddit post](https://www.reddit.com/r/ProgrammerHumor/comments/3nc531/in_case_of_fire/)

[Image source](https://instagram.com/p/8N8J8wRgPq/) | [Printable Image](http://imgur.com/IiAdxbB) | Artist: [Ákos Szokodi](https://github.com/szokodiakos)
