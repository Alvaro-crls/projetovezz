# VEZZ – Plataforma Inteligente de Gestão de Atendimentos e Filas

Sistema para clínicas e consultórios gerenciarem filas de atendimento e agendamentos de pacientes.

## Tecnologias
- PHP 7.4+ (PDO, Sessions)
- MySQL / Postgres
- Bootstrap 5
- JavaScript (AJAX)

## Estrutura (resumida)
Arquivos e pastas principais:

- `index.php`, `login.php`, `logout.php`, `cadastro.php`
- `agendamento.php`, `controle_fila.php`, `acompanhamento_fila.php`
- `assets/` (css, js, img)
- `includes/` (config, auth, functions, header, footer)
- `sql/` (script de criação do banco)

## Instalação local (XAMPP / WAMP / similar)

1. Copie a pasta do projeto para `C:\xampp\htdocs\vezz` (Windows) ou `/var/www/html/vezz` (Linux).
2. Importe o script SQL em `sql/` no seu gerenciador de banco (phpMyAdmin, pgAdmin, etc.).
3. Ajuste `includes/config.php` com as credenciais locais do banco.
4. Acesse `http://localhost/vezz/`.

## Testes & Debug

- Verifique os logs do servidor web (Apache/Nginx/PHP) para erros de conexão ou permissões.
- Para migrações em serviços como Supabase use a interface SQL ou a CLI oficial.

## Segurança

- Nunca commit `DB_PASSWORD`, `.env` ou segredos no repositório público.
- Use variáveis de ambiente/segredos do provedor de hospedagem.

## Observações

As instruções e artefatos para deploy via Docker/Render/Fly foram removidos deste repositório conforme solicitado.

Se quiser, posso procurar e remover integrações de CI/CD ou arquivos residuais relacionados a deploy.
