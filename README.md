# AES CTR

AES cipher in CTR mode.

## Installation

If [available in Hex](https://hex.pm/docs/publish), the package can be installed as:

* Add `aes_ctr` to your list of dependencies in `mix.exs`:

```elixir
def deps do
  [{:aes_ctr, "~> 0.1.0"]
end
```

* Ensure `aes_ctr_ex` is started before your application:

```elixir
def application do
  [applications: [:aes_ctr]]
end
```

## Usage

* Generate AES_128 key:

```elixir
{:ok, key} = AesCtr.generate_aes_key(:bytes)
{:ok, key_in_base64} = AesCtr.generate_aes_key(:base64)
```

## Configuration