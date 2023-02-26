# Editar as config globais dos git 
```bash
  git config --global core.editor code
```

# Alias para git 
```bash
  git config --global --edit
```

# arquivo de configuração 
```.gitconfig
[user]
	email = anderson.tec12@gmail.com
	name = Anderson Barros Silva
[core]
	editor = code --wait
[push]
	followTags = true
[alias]
	c = !git add --all && git commit -m
	s = !git status -s
	l = !git log --pretty=format:'%C(blue)%h%C(red)%d %C(white)%s - %C(cyan)%cn, %C(green)%cr'
	amend = !git add --all && git commit --amend --no-edit
	count = !git shortlog -s --grep
	t = !git tag 
```

<hr />

# Alias exemplos 

<ul>
  <li><strong> git c "mesagem" </strong> - Atalho para adicionar e comitar</li>
  <li><strong> git s </strong> - Atalho para status resumido</li>
  <li><strong> git l </strong> - Atalho para log resumido com informações personalizadas</li>
  <li><strong> git amend </strong> - Atalho para juntar commits</li>
  <li><strong> git count feat </strong> - Atalho para pegar os tipos de commits, feat, chore, bug,docs e etc</li>
  <li><strong> git t -a "1.0.0" -m "1.0.0"</strong> - Atalho para criar tags assinadas </li>
</ul>