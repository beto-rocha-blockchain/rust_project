# calc_near_x

Uma biblioteca Rust para cálculos matemáticos com operações básicas.

## Funcionalidades

- **Soma com incremento**: Adiciona 1 ao resultado da soma
- **Subtração com decremento**: Subtrai 1 do resultado da subtração (retorna 0 se o primeiro número for menor ou igual ao segundo)

## Instalação

Adicione a dependência ao seu `Cargo.toml`:

```toml
[dependencies]
calc_near_x = "0.1.1"
```

## Uso

```rust
use calc_near_x::calc_with_1;

// Soma com incremento
let resultado = calc_with_1::sum_plus_one(5, 6);
assert_eq!(resultado, 12); // 5 + 6 + 1 = 12

// Subtração com decremento
let resultado = calc_with_1::sub_less_one(6, 1);
assert_eq!(resultado, 4); // 6 - 1 - 1 = 4

// Retorna 0 se o primeiro número for menor ou igual ao segundo
let resultado = calc_with_1::sub_less_one(5, 6);
assert_eq!(resultado, 0);
```

## Documentação

Execute `cargo doc --open` para ver a documentação completa da API.

## Licença

Este projeto está licenciado sob a licença MIT - veja o arquivo [LICENSE](LICENSE) para detalhes.
