# Base-de-datosSQL
 # PostgreSQL Database Dump

This is a PostgreSQL database dump file.

- Database version: 12.9 (Ubuntu 12.9-2.pgdg20.04+1)
- Dumped by: pg_dump version 12.9 (Ubuntu 12.9-2.pgdg20.04+1)

## Table of Contents

- [Database Structure](#database-structure)
- [Data](#data)
- [Constraints](#constraints)

## Database Structure

### Tables

1. **category**
   - `category_id` INTEGER NOT NULL
   - `designer_id` INTEGER
   - `category_name` VARCHAR(200) NOT NULL
   - `name` VARCHAR(20)
   - `film` VARCHAR(40) NOT NULL

2. **city**
   - `city_id` INTEGER NOT NULL
   - `name` VARCHAR(30) NOT NULL
   - `population` NUMERIC
   - `empire_or_republic` TEXT

3. **designer**
   - `designer_id` INTEGER NOT NULL
   - `designer_name` VARCHAR(50) NOT NULL
   - `name` VARCHAR(40) NOT NULL
   - `film` VARCHAR(40) NOT NULL

4. **galaxy**
   - `galaxy_id` INTEGER NOT NULL
   - `name` VARCHAR(20) NOT NULL
   - `age` INTEGER NOT NULL
   - `population_in_millions` INTEGER
   - `empire_or_republic` VARCHAR(8)

5. **moon**
   - `moon_id` INTEGER NOT NULL
   - `name` VARCHAR(20) NOT NULL
   - `surface` INTEGER NOT NULL
   - `data` TEXT NOT NULL
   - `is_habitated` BOOLEAN

6. **planet**
   - `planet_id` INTEGER NOT NULL
   - `name` VARCHAR(20) NOT NULL
   - `surface` INTEGER NOT NULL
   - `empire_or_republic` VARCHAR(8)
   - `is_habitated` BOOLEAN

7. **star**
   - `star_id` INTEGER NOT NULL
   - `name` VARCHAR(20) NOT NULL
   - `lumen_in_millions` INTEGER
   - `is_habitated` BOOLEAN
   - `empire_or_republic` VARCHAR(8)

### Sequences

1. **category_category_id_seq**
   - Sequence for `category_id` in table `category`

2. **designer_designer_id_seq**
   - Sequence for `designer_id` in table `designer`

## Data

### category

- Marketing (Billy Gibbons, Solo)
- Special effects (Dawn D´Ambrosio, Star Wars VII)
- Catering (Mike Krasisky, Rogue One)

### city

- Abandoned Village (0, republic)
- Allyuen spaceport (5432, empire)
- Ambaril (355, free)

### designer

- Codix artifex (Imanol Asolo, A new beginning)
- The artist (George Lucas, Star Wars Saga)
- The director (Robert Rodriguez, The Bobba Fett book)

### galaxy

- Andromeda (5)
- Antennae (0)
- Backward (0)
- Black Eye (0)
- Bode´s galaxy (0)
- Butterfly (0)

### moon

- Alakatha (1, from K´vath)
- Alaris prime (1, free moon)
- Antar 4 (1, from Antar)
- Brentaal IV (2, from Brentaal)
- Cybloc (4, from Cybloc)
- Da Soocha V (2, from Da Soocha)
- Dorumaa (3, from Almas)
- Dun (3, from Onderon)
- Ebaq 9 (1, from Ebaq)
- Forestmoon of Endor (8, Endor moon)
- Gall (1, from Zhar)
- Gerrard V (2, from Gerrard)
- Jade Moon (3, from Loronar)
- Kethor (2, from Kothis)
- Kohlma (2, from Bogden)
- Kr (1, Ooribu)
- Lenico Belt (3, from Cairn)
- Lodos (3, from Elrood)
- Nar Shadaa (6, from Nal Hutta)
- Ohma D´un (2, from Naboo)

### planet

- Abafar (2)
- Agamar (4)
- Ahch-To (5)
- Ajan Kloss (12)
- Akiva (7)
- Alderaan (23)
- Aaleen (2)
- Alzoc III (4)
- Anaxes (2)
- Ando (8)
- Anoat (2)
- Atollon (5)

### star

- Lynx
- Eridanus
- Cassiopeia
- Scorpius
- Crux
- Canceer

## Constraints

- `category_name_key` (Unique constraint on `name` in table `category`)
- `category_pkey` (Primary key constraint on `category_id` in table `category`)
- `city_empire_or_republic_key` (Unique constraint on `empire_or_republic` in table `city`)
- `city_pkey` (Primary key constraint on `city_id` in table `city`)
- `designer_film_key` (Unique constraint on `film` in table `designer`)
- `designer_pkey` (Primary key constraint on `designer_id` in table `designer`)
- `galaxy_pkey` (Primary key constraint on `galaxy_id` in table `galaxy`)
- `galaxy_population_in_millions_key` (Unique constraint on `population_in_millions` in table `galaxy`)
- `moon_is_habitated_key` (Unique constraint on `is_habitated` in table `moon`)
- `moon_pkey` (Primary key constraint on `moon_id` in table `moon`)
- `planet_is_habitated_key` (Unique constraint on `is_habitated` in table `planet`)
- `planet_pkey` (Primary key constraint on `planet_id` in table `planet`)
- `star_lumen_in_millions_key` (Unique constraint on `lumen_in_millions` in table `star`)
- `star_pkey` (Primary key constraint on `star_id` in table `star`)
- `fk_designer` (Foreign key constraint referencing `designer_id` in table `designer` from `category`)

This PostgreSQL database dump is complete.

## 日本語 (Japanese)

# PostgreSQL データベースダンプ

これは PostgreSQL データベースダンプファイルです。

- データベースバージョン: 12.9 (Ubuntu 12.9-2.pgdg20.04+1)
- ダンプ作成ツール: pg_dump バージョン 12.9 (Ubuntu 12.9-2.pgdg20.04+1)

## 目次

- [データベース構造](#データベース構造)
- [データ](#データ)
- [制約](#制約)

## データベース構造

### テーブル

1. **category**
   - `category_id` INTEGER NOT NULL
   - `designer_id` INTEGER
   - `category_name` VARCHAR(200) NOT NULL
   - `name` VARCHAR(20)
   - `film` VARCHAR(40) NOT NULL

2. **city**
   - `city_id` INTEGER NOT NULL
   - `name` VARCHAR(30) NOT NULL
   - `population` NUMERIC
   - `empire_or_republic` TEXT

3. **designer**
   - `designer_id` INTEGER NOT NULL
   - `designer_name` VARCHAR(50) NOT NULL
   - `name` VARCHAR(40) NOT NULL
   - `film` VARCHAR(40) NOT NULL

4. **galaxy**
   - `galaxy_id` INTEGER NOT NULL
   - `name` VARCHAR(20) NOT NULL
   - `age` INTEGER NOT NULL
   - `population_in_millions` INTEGER
   - `empire_or_republic` VARCHAR(8)

5. **moon**
   - `moon_id` INTEGER NOT NULL
   - `name` VARCHAR(20) NOT NULL
   - `surface` INTEGER NOT NULL
   - `data` TEXT NOT NULL
   - `is_habitated` BOOLEAN

6. **planet**
   - `planet_id` INTEGER NOT NULL
   - `name` VARCHAR(20) NOT NULL
   - `surface` INTEGER NOT NULL
   - `empire_or_republic` VARCHAR(8)
   - `is_habitated` BOOLEAN

7. **star**
   - `star_id` INTEGER NOT NULL
   - `name` VARCHAR(20) NOT NULL
   - `lumen_in_millions` INTEGER
   - `is_habitated` BOOLEAN
   - `empire_or_republic` VARCHAR(8)

### シーケンス

1. **category_category_id_seq**
   - テーブル `category` の `category_id` のシーケンス

2. **designer_designer_id_seq**
   - テーブル `designer` の `designer_id` のシーケンス

## データ

(データは英語版と同じです)

## 制約

(制約は英語版と同じです)

この PostgreSQL データベースダンプは完了しました。

---

## 中文 (Chinese)

# PostgreSQL 数据库转储

这是一个 PostgreSQL 数据库转储文件。

- 数据库版本：12.9 (Ubuntu 12.9-2.pgdg20.04+1)
- 转储工具版本：pg_dump 版本 12.9 (Ubuntu 12.9-2.pgdg20.04+1)

## 目录

- [数据库结构](#数据库结构)
- [数据](#数据)
- [约束](#约束)

## 数据库结构

### 表格

1. **category**
   - `category_id` 整数 非空
   - `designer_id` 整数
   - `category_name` 可变长字符(200) 非空
   - `name` 可变长字符(20)
   - `film` 可变长字符(40) 非空

2. **city**
   - `city_id` 整数 非空
   - `name` 可变长字符(30) 非空
   - `population` 数值
   - `empire_or_republic` 文本

3. **designer**
   - `designer_id` 整数 非空
   - `designer_name` 可变长字符(50) 非空
   - `name` 可变长字符(40) 非空
   - `film` 可变长字符(40) 非空

4. **galaxy**
   - `galaxy_id` 整数 非空
   - `name` 可变长字符(20) 非空
   - `age` 整数 非空
   - `population_in_millions` 整数
   - `empire_or_republic` 可变长字符(8)

5. **moon**
   - `moon_id` 整数 非空
   - `name` 可变长字符(20) 非空
   - `surface` 整数 非空
   - `data` 文本 非空
   - `is_habitated` 布尔

6. **planet**
   - `planet_id` 整数 非空
   - `name` 可变长字符(20) 非空
   - `surface` 整数 非空
   - `empire_or_republic` 可变长字符(8)
   - `is_habitated` 布尔

7. **star**
   - `star_id` 整数 非空
   - `name` 可变长字符(20) 非空
   - `lumen_in_millions` 整数
   - `is_habitated` 布尔
   - `empire_or_republic` 可变长字符(8)

### 序列

1. **category_category_id_seq**
   - 表格 `category` 的 `category_id` 序列

2. **designer_designer_id_seq**
   - 表格 `designer` 的 `designer_id` 序列

## 数据

(数据同英文版)

## 约束

(约束同英文版)

此 PostgreSQL 数据库转储完毕。
