
# Regex - tirar espaços e caracteres especiais

str = str.replace(/[^a-z0-9-]/g, '');
Tudo entre indica o que você está procurando

- / está aqui para delimitar o seu padrão para que você tenha um para começar e outro para terminar
- [] indica o padrão que você está procurando em um caractere específico
- ^ indica que você deseja que cada caractere NÃO corresponda ao que segue a-z corresponde a qualquer caractere entre 'a' e 'z' incluído 0-9 corresponde a qualquer dígito entre '0' e '9' incluído (ou seja, qualquer dígito)
- o personagem
g no final há um parâmetro especial dizendo que você não quer que a regex pare no primeiro caractere que corresponda ao seu padrão, mas continue em toda a string

Então, sua expressão é delimitada por /antes e depois. Então aqui você diz "todo caractere que não seja uma letra, um dígito ou um '-' será removido da string".

str = str.replace(/[^a-z0-9-]/g, "");
Você pode ler como:

[^ ]: corresponder NÃO do conjunto
[^a-z0-9-]: corresponde se não a-z, 0-9ou-
/ /g: fazer combinação global