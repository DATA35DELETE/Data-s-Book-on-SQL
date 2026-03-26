# Data's Book on SQL

## SQL

### Ön Söz
- Ben kimim?
- Bu Data's Book on SQL nedir?
- Bu dokümantasyon ne öğretecek?

---

### SQL : Giriş
- **Veritabanı Nedir?**: Tanım. Kullanım Senaryoları.
- **İlişkisel Veritabanı Nedir?**: Tanım. Tablo Yapısı. Satır ve Sütun.
- **SQL Nedir?**: Tanım. Kısa Tarihçesi. Kullanım Alanları.
- **SQL Nedir?**
  - **Kısa Tarihçesi**
  - **Diğer Veritabanlarıyla Farkı**: MySQL, SQLite, MSSQL. Tablo Halinde.
  - **Kullanım Alanları**
- **SQL Kurulumu**
  - **Linux (apt)**: Kurulum. Servis Başlatma. Örnek.
  - **Windows**: Kurulum. Örnek.
  - **psql CLI**: Bağlanma. Temel Komutlar. Örnek.
  - **pgAdmin**: Kurulum. Arayüz Tanıtımı.
- **İlk Veritabanı**: CREATE DATABASE. Bağlanma. Örnek.

---

### SQL : Veri Tipleri
- **Veri Tipi Nedir?**: Tanım. Neden Önemli?
- **Sayısal Tipler**
  - **SMALLINT**: Tanım. Örnek.
  - **INTEGER**: Tanım. Örnek.
  - **BIGINT**: Tanım. Örnek.
  - **DECIMAL / NUMERIC**: Tanım. Hassasiyet. Örnek.
  - **REAL / DOUBLE PRECISION**: Tanım. Örnek.
  - **SERIAL / BIGSERIAL**: Tanım. Auto-increment. Örnek.
- **Metin Tipleri**
  - **CHAR(n)**: Tanım. Örnek.
  - **VARCHAR(n)**: Tanım. CHAR ile Farkı. Örnek.
  - **TEXT**: Tanım. Örnek.
- **Tarih ve Zaman Tipleri**
  - **DATE**: Tanım. Örnek.
  - **TIME**: Tanım. Örnek.
  - **TIMESTAMP**: Tanım. Örnek.
  - **TIMESTAMPTZ**: Tanım. Timezone. Örnek.
  - **INTERVAL**: Tanım. Örnek.
- **Boolean**: Tanım. TRUE / FALSE / NULL. Örnek.
- **UUID**: Tanım. gen_random_uuid(). Örnek.
- **JSON ve JSONB**: Tanım. Farkları. Örnek.
- **ARRAY**: Tanım. Örnek.
- **NULL**: Tanım. NULL ile Karşılaştırma. Dikkat Edilecekler.

---

### SQL : Tablo İşlemleri
- **Tablo Nedir?**: Tanım. Şema (Schema) Kavramı.
- **Tablo Oluşturma (CREATE TABLE)**: Tanım. Örnek.
- **Tablo Silme (DROP TABLE)**: Tanım. IF EXISTS. Örnek.
- **Tablo Değiştirme (ALTER TABLE)**
  - **Sütun Ekleme**: ADD COLUMN. Örnek.
  - **Sütun Silme**: DROP COLUMN. Örnek.
  - **Sütun Tipi Değiştirme**: ALTER COLUMN. Örnek.
  - **Tablo Adı Değiştirme**: RENAME TO. Örnek.
- **Geçici Tablo (TEMP TABLE)**: Tanım. Örnek.
- **Tablo Kopyalama**: CREATE TABLE AS. Örnek.

---

### SQL : Kısıtlamalar (Constraints)
- **Kısıtlama Nedir?**: Tanım. Kullanım Senaryoları.
- **PRIMARY KEY**: Tanım. Composite PK. Örnek.
- **FOREIGN KEY**: Tanım. ON DELETE / ON UPDATE Seçenekleri. Örnek.
- **UNIQUE**: Tanım. Örnek.
- **NOT NULL**: Tanım. Örnek.
- **CHECK**: Tanım. Örnek.
- **DEFAULT**: Tanım. Örnek.
- **Kısıtlama Ekleme / Silme**: ALTER TABLE ile. Örnek.

---

### SQL : Veri İşlemleri (DML)
- **DML Nedir?**: Tanım. INSERT, UPDATE, DELETE, SELECT.
- **Veri Ekleme (INSERT)**
  - **Tek Satır Ekleme**: Tanım. Örnek.
  - **Çoklu Satır Ekleme**: Tanım. Örnek.
  - **INSERT ... RETURNING**: Tanım. Örnek.
  - **ON CONFLICT (Upsert)**: Tanım. Örnek.
- **Veri Güncelleme (UPDATE)**
  - **Temel UPDATE**: Tanım. Örnek.
  - **UPDATE ... RETURNING**: Tanım. Örnek.
  - **JOIN ile UPDATE**: Tanım. Örnek.
- **Veri Silme (DELETE)**
  - **Temel DELETE**: Tanım. Örnek.
  - **DELETE ... RETURNING**: Tanım. Örnek.
  - **TRUNCATE**: Tanım. DELETE ile Farkı. Örnek.

---

### SQL : Sorgulama (SELECT)
- **SELECT Nedir?**: Tanım. Temel Yapı.
- **Temel SELECT**: Tanım. Örnek.
- **WHERE**: Tanım. Koşullar. Örnek.
  - **AND / OR / NOT**: Tanım. Örnek.
  - **BETWEEN**: Tanım. Örnek.
  - **IN / NOT IN**: Tanım. Örnek.
  - **LIKE / ILIKE**: Tanım. Wildcard. Örnek.
  - **IS NULL / IS NOT NULL**: Tanım. Örnek.
- **ORDER BY**: Tanım. ASC / DESC. Örnek.
- **LIMIT ve OFFSET**: Tanım. Sayfalama. Örnek.
- **DISTINCT**: Tanım. Örnek.
- **Alias (AS)**: Sütun ve Tablo Alias. Örnek.

---

### SQL : Fonksiyonlar ve Operatörler
- **Aggregate Fonksiyonlar**: Tanım. Kullanım Senaryoları.
  - **COUNT**: Tanım. Örnek.
  - **SUM**: Tanım. Örnek.
  - **AVG**: Tanım. Örnek.
  - **MIN / MAX**: Tanım. Örnek.
- **String Fonksiyonları**: UPPER, LOWER, LENGTH, TRIM, CONCAT, SUBSTRING. Örnek.
- **Sayısal Fonksiyonlar**: ROUND, FLOOR, CEIL, ABS, MOD. Örnek.
- **Tarih Fonksiyonları**: NOW(), CURRENT_DATE, AGE(), DATE_PART(), TO_CHAR(). Örnek.
- **Koşullu İfadeler**
  - **CASE WHEN**: Tanım. Örnek.
  - **COALESCE**: Tanım. NULL yönetimi. Örnek.
  - **NULLIF**: Tanım. Örnek.
- **Tip Dönüşümü (CAST)**: Tanım. :: Operatörü. Örnek.

---

### SQL : Gruplama
- **GROUP BY**: Tanım. Örnek.
- **HAVING**: Tanım. WHERE ile Farkı. Örnek.
- **GROUPING SETS**: Tanım. Örnek.
- **ROLLUP**: Tanım. Örnek.
- **CUBE**: Tanım. Örnek.

---

### SQL : JOIN İşlemleri
- **JOIN Nedir?**: Tanım. İlişkisel Mantık.
- **INNER JOIN**: Tanım. Örnek.
- **LEFT JOIN**: Tanım. Örnek.
- **RIGHT JOIN**: Tanım. Örnek.
- **FULL OUTER JOIN**: Tanım. Örnek.
- **CROSS JOIN**: Tanım. Örnek.
- **SELF JOIN**: Tanım. Örnek.
- **Çoklu JOIN**: Tanım. Örnek.

---

### SQL : Alt Sorgular (Subqueries)
- **Alt Sorgu Nedir?**: Tanım. Kullanım Senaryoları.
- **WHERE'de Alt Sorgu**: Tanım. Örnek.
- **FROM'da Alt Sorgu**: Türetilmiş Tablo. Örnek.
- **SELECT'te Alt Sorgu**: Skalar Alt Sorgu. Örnek.
- **EXISTS / NOT EXISTS**: Tanım. Örnek.
- **ANY / ALL**: Tanım. Örnek.
- **Correlated Subquery**: Tanım. Örnek.

---

### SQL : CTE (Common Table Expressions)
- **CTE Nedir?**: Tanım. Avantajları.
- **WITH Kullanımı**: Tanım. Örnek.
- **Çoklu CTE**: Tanım. Örnek.
- **Recursive CTE**: Tanım. Örnek. Kullanım Senaryoları.
- **CTE vs Alt Sorgu**: Farkları. Ne Zaman Hangisi? Tablo Halinde.

---

### SQL : Window Fonksiyonları
- **Window Fonksiyonu Nedir?**: Tanım. GROUP BY ile Farkı.
- **OVER ve PARTITION BY**: Tanım. Örnek.
- **ORDER BY ile Window**: Tanım. Örnek.
- **Sıralama Fonksiyonları**
  - **ROW_NUMBER()**: Tanım. Örnek.
  - **RANK()**: Tanım. Örnek.
  - **DENSE_RANK()**: Tanım. Örnek.
  - **NTILE()**: Tanım. Örnek.
- **Kaydırma Fonksiyonları**
  - **LAG()**: Tanım. Örnek.
  - **LEAD()**: Tanım. Örnek.
  - **FIRST_VALUE() / LAST_VALUE()**: Tanım. Örnek.
- **Kümülatif Aggregate**: SUM() OVER, AVG() OVER. Örnek.

---

### SQL : İndeksler
- **İndeks Nedir?**: Tanım. Performans Etkisi. Kullanım Senaryoları.
- **B-Tree İndeks**: Tanım. Varsayılan. Örnek.
- **Hash İndeks**: Tanım. Örnek.
- **GIN İndeks**: Tanım. JSON ve Array. Örnek.
- **GiST İndeks**: Tanım. Örnek.
- **Composite İndeks**: Tanım. Örnek.
- **Partial İndeks**: Tanım. Örnek.
- **Unique İndeks**: Tanım. Örnek.
- **İndeks Silme**: DROP INDEX. Örnek.
- **EXPLAIN / EXPLAIN ANALYZE**: Sorgu Planı Okuma. Örnek.

---

### SQL : View'lar
- **View Nedir?**: Tanım. Avantajları. Kullanım Senaryoları.
- **View Oluşturma (CREATE VIEW)**: Tanım. Örnek.
- **View Güncelleme**: Updatable View. Örnek.
- **View Silme (DROP VIEW)**: Tanım. Örnek.
- **Materialized View**: Tanım. Normal View ile Farkı. Örnek.
  - **REFRESH MATERIALIZED VIEW**: Tanım. Örnek.

---

### SQL : Stored Procedure ve Fonksiyonlar
- **PL/pgSQL Nedir?**: Tanım. Kullanım Senaryoları.
- **Fonksiyon Oluşturma (CREATE FUNCTION)**: Tanım. Örnek.
- **Parametreli Fonksiyon**: IN / OUT / INOUT. Örnek.
- **Return Türleri**: RETURNS TABLE. RETURNS SETOF. Örnek.
- **Stored Procedure (CREATE PROCEDURE)**: Tanım. Fonksiyon ile Farkı. Örnek.
- **Değişkenler ve Kontrol Yapıları**
  - **DECLARE**: Tanım. Örnek.
  - **IF / ELSIF / ELSE**: Tanım. Örnek.
  - **LOOP / FOR / WHILE**: Tanım. Örnek.
- **Exception Handling**: BEGIN ... EXCEPTION. Örnek.
- **Fonksiyon Silme**: DROP FUNCTION. Örnek.

---

### SQL : Trigger'lar
- **Trigger Nedir?**: Tanım. Kullanım Senaryoları.
- **Trigger Oluşturma**: CREATE TRIGGER. Örnek.
- **BEFORE / AFTER / INSTEAD OF**: Tanım. Farkları. Örnek.
- **ROW vs STATEMENT Level**: Tanım. Örnek.
- **NEW ve OLD**: Tanım. Örnek.
- **Trigger Fonksiyonu**: RETURNS TRIGGER. Örnek.
- **Trigger Silme**: DROP TRIGGER. Örnek.

---

### SQL : Transaction Yönetimi
- **Transaction Nedir?**: Tanım. ACID. Kullanım Senaryoları.
- **BEGIN / COMMIT / ROLLBACK**: Tanım. Örnek.
- **SAVEPOINT**: Tanım. Kısmi Geri Alma. Örnek.
- **İzolasyon Seviyeleri**: READ COMMITTED, REPEATABLE READ, SERIALIZABLE. Tablo Halinde.
- **Deadlock**: Tanım. Nasıl Oluşur? Nasıl Önlenir? Örnek.
- **Locking**: ROW LOCK. TABLE LOCK. FOR UPDATE. Örnek.

---

### SQL : JSON ve JSONB İşlemleri
- **JSON vs JSONB**: Tanım. Farkları. Ne Zaman Hangisi?
- **JSON Ekleme ve Okuma**: Tanım. Örnek.
- **JSON Operatörleri**: ->, ->>, #>, #>>. Tanım. Örnek.
- **JSON Fonksiyonları**: json_each, json_array_elements, jsonb_set. Örnek.
- **JSONB İndeksleme**: GIN ile. Örnek.
- **JSONB Güncelleme**: jsonb_set. || operatörü. Örnek.

---

### SQL : Şema ve Veritabanı Yönetimi
- **Şema (Schema) Nedir?**: Tanım. search_path. Örnek.
- **Şema Oluşturma / Silme**: CREATE SCHEMA. DROP SCHEMA. Örnek.
- **Kullanıcı ve Rol Yönetimi**
  - **CREATE ROLE / USER**: Tanım. Örnek.
  - **GRANT / REVOKE**: Tanım. Örnek.
  - **Tablo Bazlı Yetkilendirme**: SELECT, INSERT, UPDATE, DELETE. Örnek.
- **Veritabanı Oluşturma / Silme**: CREATE DATABASE. DROP DATABASE. Örnek.
- **Bağlantı Yönetimi**: pg_hba.conf. Örnek.

---

### SQL : Performans ve Optimizasyon
- **Performans Nedir?**: Tanım. Darboğaz Analizi.
- **EXPLAIN ve EXPLAIN ANALYZE**: Sorgu Planı. Maliyet. Örnek.
- **Slow Query Tespiti**: pg_stat_statements. Örnek.
- **Vakumlama (VACUUM)**: Tanım. AUTOVACUUM. Örnek.
- **ANALYZE**: Tanım. İstatistik Güncelleme. Örnek.
- **Bağlantı Havuzu (Connection Pooling)**: PgBouncer. Tanım. Örnek.
- **Partition (Tablo Bölümleme)**: Tanım. Range, List, Hash. Örnek.
- **Parallel Query**: Tanım. Örnek.

---

### SQL : Yedekleme ve Geri Yükleme
- **Yedekleme Nedir?**: Tanım. Kullanım Senaryoları.
- **pg_dump**: Tanım. Örnek.
  > Seçenekler
- **pg_dumpall**: Tanım. pg_dump ile Farkı. Örnek.
- **pg_restore**: Tanım. Örnek.
- **psql ile Geri Yükleme**: Tanım. Örnek.
- **Sürekli Arşivleme (WAL)**: Tanım. Point-in-Time Recovery. Örnek.

---

### SQL : Replikasyon
- **Replikasyon Nedir?**: Tanım. Kullanım Senaryoları.
- **Streaming Replikasyon**: Tanım. Primary / Standby. Örnek.
- **Logical Replikasyon**: Tanım. Streaming ile Farkı. Örnek.
- **Hot Standby**: Tanım. Örnek.
- **Failover**: Tanım. Örnek.