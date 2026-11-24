# PAINEL-DE-INSUCESSO-
O PAINEL DE INSUCESSO está pronto em painel-de-insucesso.html, num arquivo único que abre direto no navegador ou pode ir para o GitHub Pages. Eu não abri nem testei o arquivo.

Login: no primeiro acesso, quem se cadastrar vira administrador. Depois disso, só o administrador cria usuários, redefine senhas ou remove contas. As senhas são guardadas com hash.
Registro vinculado ao login: cada registro grava o responsável logado, e o usuário comum só vê e edita os próprios. O administrador vê tudo e filtra por pessoa.
Campos do registro: data, responsável, SVC (padrão SRJ15), ID do pacote, MLP (transportadora), nome do driver, motivo e situação final. Há opção para manter MLP, driver, motivo e situação depois de salvar, para agilizar o lançamento em lote. O sistema avisa se o ID do pacote já foi registrado.
Relatórios: com filtros por data, MLP, motivo, situação, responsável e busca, o PDF sai com cabeçalho, resumos e tabela, e o Excel traz as abas "Registros" e "Resumo".
Listas: montei as de MLP, motivos e situação final a partir dos seus prints, sem as duplicatas de grafia (Comercio Fechado, ON TIME SERVICOS). O motivo "PACOTE ENVIADO …" estava cortado no print, então coloquei "Pacote enviado"; confira o texto completo. O administrador edita as listas na aba Administração.
Paleta Kuehne+Nagel: usei azul-marinho, azul-céu e fundo azul-claro. As cores são aproximadas, porque não achei os HEX oficiais. Se tiver o manual da marca, troque as cores no bloco :root do CSS.

Os dados ficam salvos no navegador de quem usa, ou seja, cada computador tem a sua base. Para várias pessoas lançarem num mesmo painel, preciso ligar o painel a uma planilha do Google com Apps Script, como na Central de Reatribuição. Enquanto isso, o botão "Baixar backup (JSON)" na aba Administração serve de cópia de segurança.
