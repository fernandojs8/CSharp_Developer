# C# Developer — fundamentos e orientação a objetos

Trilha de estudos da **Alura** com exercícios de C# e .NET Framework. O domínio didático ByteBank acompanha a evolução de classes e encapsulamento para herança, interfaces, exceções, bibliotecas, coleções e LINQ.

## Roteiro do repositório

| Módulo |
| --- |
| [01 — PrimeirosPassos](01_PrimeirosPassos) |
| [02 — IntroducaoAOrientacaoAObjetos](02_IntroducaoAOrientacaoAObjetos) |
| [03 — EntendendoHerancaEInterface](03_EntendendoHerancaEInterface) |
| [04 — EntendendoExcecoes](04_EntendendoExcecoes) |
| [05 — DLLsLib_NuGet](05_DLLsLib_NuGet) |
| [06 — StringsExpressoesRegularesEAClasseObject](06_StringsExpressoesRegularesEAClasseObject) |
| [07 — ArraysETiposGenericos](07_ArraysETiposGenericos) |
| [08 — ListLambdaLINQ](08_ListLambdaLINQ) |
| [09 — IOStreams](09_IOStreams) |
| [10 — Collections](10_Collections) |
| [11 — Collections_2](11_Collections_2) |

As pastas representam etapas independentes do aprendizado. Há várias soluções e versões do ByteBank; elas não formam um único sistema bancário integrado. O diretório `07_ArraysETiposGenericos` contém uma solução para o módulo de arrays, além de existir uma pasta histórica com espaços no nome.

## Competências demonstradas

- Sintaxe, tipos, condições, loops e escopo.
- Modelagem orientada a objetos, herança, polimorfismo e contratos por interfaces.
- Tratamento de exceções e organização em bibliotecas de classes.
- Strings, expressões regulares, arrays e tipos genéricos.
- Consultas com lambdas/LINQ, leitura e escrita com streams e coleções como pilhas e filas.

Nos módulos com `ByteBank.Modelos` e `ByteBank.SistemaAgencia`, a separação entre biblioteca de modelos e aplicação console permite explorar referências entre projetos. Essa organização é didática; não representa uma arquitetura de serviços ou integração com um banco financeiro real.

## Tecnologias e execução

Os projetos inspecionados usam **C# e .NET Framework 4.6.1**, com arquivos de projeto no formato clássico do Visual Studio. Para reproduzir a configuração original, use Windows, Visual Studio com ferramentas de desenvolvimento .NET desktop e o targeting pack compatível com o framework alvo. O comando `dotnet run` de projetos SDK modernos não é uma instrução universal para estas soluções.

```powershell
git clone https://github.com/fernandojs8/CSharp_Developer.git
Set-Location CSharp_Developer
Start-Process "03_EntendendoHerancaEInterface/ByteBank.sln"
```

No Visual Studio:

1. Restaure os pacotes NuGet quando solicitados.
2. Selecione o projeto console desejado como projeto de inicialização.
3. Compile a solução e execute com Ctrl+F5; acompanhe as operações demonstradas no console.
4. Para outro módulo, abra a solução daquela pasta e leia seu `Program.cs` e eventual README local.

Para os exercícios de streams, confira os caminhos dos arquivos de entrada e a pasta de trabalho antes de executar. Referências externas ou pacotes antigos podem exigir ajustes no ambiente; documente esses ajustes separadamente de uma atualização do código.

## Testes e validação

Não foi identificada suíte automatizada com xUnit, NUnit ou MSTest. Os programas console são exemplos para exploração manual, não evidências de cobertura de testes.

Roteiro manual sugerido: executar um módulo, observar a saída, alterar entradas e comparar o comportamento de tipos/classes, exceções ou coleções estudadas. **Build e execução não foram realizados nesta revisão**, que se limitou à leitura de projetos e fontes; o ambiente de análise não possui `dotnet`.

## Limitações e próximos passos

- Framework e formato de projeto históricos; a reprodução depende do ambiente compatível.
- Exemplos duplicados por etapa fazem parte da progressão do curso e não devem ser compilados como uma solução única.
- O ByteBank é uma simulação educacional; não há integração bancária real ou evidência de operação em produção.
- Evoluções propostas: migrar um módulo por vez para formato SDK, adicionar testes de regras de domínio e IO, organizar dados de exemplo e criar CI de build/testes.
- Para o portfólio, o melhor próximo artefato é um módulo modernizado com testes e resultado de pipeline verificável. Cloud pode ser explorada em um projeto web derivado, identificado como trabalho novo.

## Origem e licença

[Formação C# da Alura](https://www.alura.com.br/carreira-desenvolvedor-csharp), referência histórica da trilha. Código sob [MIT](LICENSE).
