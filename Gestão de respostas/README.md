# Sistema de Gestão de Respostas CASSI (SiGRC)

## 1. Visão geral

> ### Domínio
>
> A caixa de e-mail da divisão recebe algumas mensagens que precisam de acompanhamento. O sistema objeto deste documento visa prover controle sobre a situação dessas mensagens.

## 2. UX/UI

## 3. Persistência

> ### Banco de dados
> Os registros do sistema são essencialmente mantidos **`localmente`** em um banco de dados não relacional.
>
> ### Exportação de dados
> Cada instância em operação busca um arquivo estruturado com conteúdo **`serializado`** localizado no mesmo diretório do executável.

## 4. Distribuição interna

> ### Dentro de uma divisão
>
> Assumindo que em algum momento o sistema poderá **`receber`** acessos concorrentes dentro da sua esfera de execução, é necessário que os **`colaboradores de uma mesma divisão`** tenham acesso aos mesmos dados. Para que isso ocorra, **`todas as instâncias do SiGRC em execução devem apontar para o mesmo banco de dados local`** isso pode ser feito especificando o caminho completo do banco de dados nas configurações do SiGRC.

## 5. Requisitos

> ### Execução
> Para que o SiGRC seja executado, é necessário que o sistema tenha o  **`vc_redist140.dll`** instalado.
>