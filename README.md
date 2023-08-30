# Swimlane API Client

![Alt text](<https://img.shields.io/badge/swimlane-11.12.x-green>)

This is a rust client for the Swimlane API. Please note that this isn't anywhere near completion. Swimlane's API documentation is not complete, so this client is not complete. I will be adding to this as I need to use more of the API. If you need something that isn't here, please feel free to open an issue or a pull request.

## Usage

Add this to your `Cargo.toml`:

```toml
[dependencies]
swimlane = "0.1.0"
```

## Example

```rust
use swimlane::Swimlane;

fn main() {
    let client = Swimlane::new("https://swimlane.example.com", "api_key");
    client.health_ping().unwrap();
}
```
