# Tailwind (versão 2.1.4)

###   Instale o Tailwind via npm
Comando para a instalação do Tailwind via npm:
```shell
npm install -D tailwindcss@latest postcss@latest autoprefixer@latest
```

Caso queira personalizar sua instalação tailwind, gere um arquivo de config para o seu projeto com o comando:
```shell
npx tailwindcss init
```

Crie um arquivo CSS se você ainda não tiver um e use a diretiva para injetar o Tailwind's e estilos, após isso adicione no seu arquivo:

 - @tailwind base; 
 - @tailwind components; 
 - @tailwind utilities;

 Para o vento de cauda que trocará essas diretivas no tempo de compilação com todos os estilos gerados com base no seu sistema de design configurado.

### Usando Tailwind without PostCSS

*O Tailwind without PostCSS requer node.js 12.13.0 ou superior.*

Para projetos simples você pode usar a ferramenta TAILwind CLI para gerar seu CSS sem configurar o PostCSS ou até mesmo instalar o Tailwind como uma dependência com o comando a baixo:
```shell
npx tailwindcss-cli@latest build Tailwind.css -o style.css
```
Isso criará um arquivo com base na configuração padrão do Tailwind e adicionará automaticamente quaisquer prefixos de fornecedor necessários.

Agora você pode puxar este arquivo em seu HTML como qualquer outra folha de estilo!