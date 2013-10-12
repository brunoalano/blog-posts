# Heroku ou Elastic Beanstalk
- Bruno Alano
- brunoalano
- 2013/07/06
- PaaS
- published

Nestes últimos dias andei fazendo alguns testes para escolher um bom proveador de **PaaS** para a Pinsell. Atualmente existem diversas, como: AppFog, Openshift, Heroku, Elastic Beanstalk, Nodester e Pandorabox. Claro, existem muitos outros, mas são os que eu lembro.

De início posso eliminar o Pandorabox, pois oferece suporte apenas a PHP, e a API está desenvolvida em Ruby. O Nodester, como o nome sugere, apenas para Node.js. Ambos, são excelentes no que fazem, e com certeza, se eu estiver utilizando alguma das duas linguagens, usaria estes serviços.

Appfog, em alguns dias de teste, não sei se foi coincidência, mas estava instável devido as mudanças de datacenters, e também pelo motivo de eu ter alocado meu serviço no Rackspace, e 3 dias depois cancelaram a parceria com a empresa, e sendo assim, tive que migrar para outro DC.

Openshift, mantido pela grande Redhat, é um bom serviço. Muitos artigos, mas sinto falta de uma documentação simples e organizada.

No final, fiquei entre Heroku e Amazon Elastic Beanstalk. Vou citar alguns pontos positivos e negativos deles.

**Heroku**: Deploy através do Git como standard, fácil configuração (você não precisa definir que linguagem ou framework está utilizando na hora do deploy), muitos addons, porém, preço relativamente alto e timeout de 30s (faz sentido ter este timeout, porém, deveria ser configurável).

**Amazon Elastic Beanstalk**: DCs em São Paulo (e muitos outros lugares), preço baixo, muito customizável, porém, a instalação torna-se mais complexa do que a do Heroku, o deploy padrão é através de Zip ou a toolbet deles.

No final de tudo, optei pela Amazon, principalmente pelo fato do servidor estar alocado em São Paulo, e já integrado com outros serviços que já tenho com eles.
