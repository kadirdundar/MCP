# 🔁 MCP Reverse String Server

Bu proje, C# ve .NET kullanılarak geliştirilen basit bir Model Context Protocol (MCP) sunucusudur. Sunucu, kullanıcıdan alınan string ifadeleri tersine çevirerek geri döndürür. Bu, MCP'nin temel işlevselliğini ve C# ile nasıl entegre edilebileceğini gösteren giriş seviyesi bir örnektir.

## 🚀 Özellikler

- MCP protokolü ile uyumlu basit bir sunucu
- Kullanıcıdan alınan string ifadeleri tersine çevirme işlevi
- Kolay kurulum ve çalıştırma

## 🛠️ Kurulum

1. **Depoyu Klonlayın:**
   ```bash
   git clone https://github.com/kullaniciadi/mcp-reverse-string-server.git
   cd mcp-reverse-string-server
   ```

2. **Gerekli NuGet Paketlerini Yükleyin:**
   Proje dizininde aşağıdaki komutu çalıştırın:
   ```bash
   dotnet restore
   ```

3. **Projeyi Derleyin ve Çalıştırın:**
   ```bash
   dotnet run
   ```
   Sunucu, MCP istemcilerinden gelen istekleri dinlemeye başlayacaktır.

## ⚙️ Kullanım

Sunucu çalıştırıldığında, MCP istemcileri aşağıdaki gibi bir istek göndererek string ifadeleri tersine çevirebilir:

```json
{
  "method": "ReverseString",
  "params": {
    "input": "Merhaba Dünya"
  }
}
```

Sunucu, aşağıdaki gibi bir yanıt döndürecektir:

```json
{
  "result": "aynüD abahreM"
}
```

## 📁 Proje Yapısı

- `Program.cs`: Sunucunun başlangıç noktası ve yapılandırması
- `ReverseTool.cs`: String tersine çevirme işlevini içeren sınıf

## 📚 Kaynaklar

- [Model Context Protocol (MCP) Resmi Dokümantasyonu](https://modelcontextprotocol.io/docs/)
- [MCP C# SDK GitHub Deposu](https://github.com/modelcontextprotocol/csharp-sdk)

## 🤝 Katkıda Bulunun

Katkılarınızı memnuniyetle karşılıyoruz! Lütfen bir [issue](https://github.com/kullaniciadi/mcp-reverse-string-server/issues) açın veya bir pull request gönderin.

## 📄 Lisans

Bu proje MIT lisansı altında lisanslanmıştır. Daha fazla bilgi için `LICENSE` dosyasına bakın.

