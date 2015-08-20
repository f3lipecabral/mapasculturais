# Mapas Culturais
Em julho de 2013, agentes culturais de vários países da América Latina e do Brasil se reuniram para discutir a criação de uma ferramenta de mapeamento de iniciativas culturais e gestão cultural. Desse encontro surgiram as bases para a criação de Mapas Culturais, um software livre que permite o aprimoramento da gestão cultural dos municípios e estados.

Mapas Culturais é uma plataforma colaborativa que reúne informações sobre agentes, espaços, eventos e projetos culturais, fornecendo ao poder público uma radiografia da área de cultura e ao cidadão um mapa de espaços e eventos culturais da região. A plataforma está alinhada ao Sistema Nacional de Informação e Indicadores Culturais do Ministério da Cultura (SNIIC) e contribui para a realização de alguns dos objetivos do Plano Nacional de Cultura.

A plataforma já está em uso, por exemplo, no município de São Paulo (http://spcultura.prefeitura.sp.gov.br/) e no estado do Rio Grande do Sul (http://mapa.cultura.rs.gov.br/).

### Travis Build Status

[![Build Status](https://secure.travis-ci.org/hacklabr/mapasculturais.png)](http://travis-ci.org/hacklabr/mapasculturais)

### Issue Tracker

Stories: [![Stories in Dev Ready](https://badge.waffle.io/hacklabr/mapasculturais.png?label=status:dev-ready)](https://waffle.io/hacklabr/mapasculturais) for Development, [![Stories in Test Ready](https://badge.waffle.io/hacklabr/mapasculturais.png?label=status:test-ready)](https://waffle.io/hacklabr/mapasculturais) for Test, [![Stories in Deploy Ready](https://badge.waffle.io/hacklabr/mapasculturais.png?label=status:tested)](https://waffle.io/hacklabr/mapasculturais) for Deploy

### Documentação 
- [Entidades dos Mapas Culturais](doc/entidades.md)
- [API](doc/api.md)
- [Guia do desenvolvedor](doc/developer-guide.md)
- [Deploy no Ubuntu 14.04 com nginx e php-fpm](doc/deploy-ubuntu-14.04.md)
- [Importação de arquivos de dados geoespaciais (Shapefiles)](doc/shapefiles.md)

### Requisitos para Instalação
- PHP >= 5.4
- Extensões PHP:
  - php5-gd
  - php5-cli
  - php5-json
  - php5-curl
  - php5-pgsql
  - php-apc
  - Zip extension enabled in php.ini
- Composer
```shell
    curl -sS https://getcomposer.org/installer | php
    sudo mv composer.phar /usr/local/bin/composer
```
- PostgreSQL >= 9.3
- Postgis Contrib (for Unaccent extension)
- Postgis >= 2.1
-  PostgreSQL Postgis Scripts

Em distribuições GNU/Linux baseadas em Debian:
```shell
sudo apt-get install php5 php5-gd php5-cli php5-json php5-curl php5-pgsql php-apc postgresql postgresql-contrib postgis postgresql-9.3-postgis-2.1 postgresql-9.3-postgis-2.1-scripts
```
- Node.JS >= 0.10
  - NPM
  - UglifyJS
  - UglifyCSS
```shell
sudo npm install -g uglify-js uglifycss autoprefixer
```
- Ruby  >= 1.9.3
  - SASS
```shell
sudo gem install sass
```
### Suporte
[![Gitter](https://badges.gitter.im/Join Chat.svg)](https://gitter.im/hacklabr/mapasculturais?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)

Lista de discussão: https://groups.google.com/forum/?hl=en#!forum/mapas-culturais

# License - AGPLv3

    This program is free software: you can redistribute it and/or modify
    it under the terms of the GNU Affero General Public License as
    published by the Free Software Foundation, either version 3 of the
    License, or (at your option) any later version.

    This program is distributed in the hope that it will be useful,
    but WITHOUT ANY WARRANTY; without even the implied warranty of
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    GNU Affero General Public License for more details.

    You should have received a copy of the GNU Affero General Public License
    along with this program.  If not, see LICENSE file here or 
    [AGPLv3](http://www.gnu.org/licenses/agpl-3.0.html).
