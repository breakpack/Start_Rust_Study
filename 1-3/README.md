**Cargo 사용**

**명령어 이용**
    $ cargo new hello_cargo --bin
        -> hello_cargo라는 실행가능한 바이너리 생성(--bin인자를 이용)

    $ cd hello_cargo

**Cargo.toml**
- TOML (Tom’s Obvious, Minimal Language) 포맷으로 작성되었는데, 이것이 Cargo의 환경설정 포맷임
- [package]은 이후의 문장들이 패키지 환경설정이라는 것을 나타내는 섹션의 시작지점
- [dependencies]은 여러분 프로젝트의 의존성들의 리스트를 적을 수 있는 섹션의 시작점

- Rust의 코드 패키지는 크레이트(Crate)라고 부름

- 코딩할때 코드를 src 디렉토리로 옮기고 적합한 Cargo.toml 파일을 생성

**build**
    $ cargo build
- build는 Cargo.toml파일이 있는 디렉토리에서 실행 -> target/debug/hello_cargo

**excute**
    $ cargo run
- ./hello_cargo로도 실행가능

**compile check**
    $ cargo check
- 실행파일 생성은 안함

**release build**
    $ cargo build --release