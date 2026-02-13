# O que significa `MZ\x90`?

`MZ` são os dois primeiros bytes (`4D 5A`) de muitos executáveis do Windows.
Esse par é a assinatura do formato **DOS MZ**, que também aparece no início de
arquivos **PE** (`.exe`, `.dll`) modernos.

O `\x90` que pode aparecer em seguida é o byte hexadecimal `90`, que em x86
representa a instrução **NOP** (*no operation*). Ver `MZ\x90` em bytes iniciais
normalmente só indica que você está olhando o começo de um executável.

## Em resumo

- `MZ` => assinatura de executável DOS/Windows.
- `\x90` => byte comum em código x86 (NOP).
- `MZ\x90` => início típico de um binário executável no ecossistema Windows.
