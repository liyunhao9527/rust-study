# Rust 学习项目

## Cargo 常用命令

### 1. 项目管理命令

```bash
# 创建新项目
cargo new project_name

# 创建新库项目
cargo new --lib library_name

# 在当前目录初始化 Cargo 项目
cargo init
```

### 2. 编译和运行命令

```bash
# 编译项目（调试模式）
cargo build

# 编译项目（发布模式，优化性能）
cargo build --release

# 编译并立即运行项目
cargo run

# 运行指定的二进制目标
cargo run --bin chapter_01_basics

# 运行指定的示例
cargo run --example example_name
```

### 3. 检查和格式化命令

```bash
# 快速检查代码，不生成可执行文件（检查编译错误）
cargo check

# 格式化代码（需要安装 rustfmt）
cargo fmt

# 检查代码风格问题（使用 Clippy）
cargo clippy
```

### 4. 测试命令

```bash
# 运行所有测试
cargo test

# 运行指定测试
cargo test test_name

# 显示测试输出（即使测试通过）
cargo test -- --nocapture
```

### 5. 文档和帮助命令

```bash
# 生成项目文档（依赖包文档）
cargo doc

# 生成文档并在浏览器中打开
cargo doc --open

# 查看命令帮助
cargo help
cargo build --help
```

### 6. 依赖管理命令

```bash
# 添加依赖包
cargo add package_name

# 添加特定版本的依赖
cargo add package_name@1.0.0

# 更新依赖
cargo update
```

### 7. 清理和调试命令

```bash
# 删除编译生成的文件
cargo clean

# 显示详细的编译信息
cargo build -vv

# 生成并打开文档
cargo doc --open
```

## 常用 Rustc 命令

```bash
# 查看 Rust 版本
rustc --version

# 编译单个 Rust 文件
rustc main.rs

# 查看可用的编译选项
rustc --help
```

## 项目结构

- `chapter_01_basics/` - 第一章：Rust 基础
  - `src/main.rs` - 主程序文件
  - `Cargo.toml` - 项目配置文件
