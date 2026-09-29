# Glossa

**Tiếng Việt** · [English](#english)

Dịch giọng nói trực tiếp trên máy tính: Glossa nghe âm thanh hệ thống hoặc micro và hiện bản dịch
ngay khi người nói đang nói — cho cuộc họp, video, livestream hay bài giảng.

Repo này chỉ chứa các bản phát hành của Glossa và là nơi app tự kiểm tra cập nhật.

## Tải về

Vào [Releases mới nhất](https://github.com/CongThang1597/glossa-releases/releases/latest) và chọn:

| Hệ điều hành | File |
|---|---|
| macOS 13 trở lên, chip Apple (M1 trở lên) | `Glossa_<phiên bản>_aarch64.dmg` |
| Windows 10 / 11 (64-bit) | `Glossa_<phiên bản>_x64-setup.exe` (hoặc `.msi`) |

Sau lần cài đầu, Glossa tự báo khi có bản mới — bấm **Cập nhật** là xong, không cần tải lại.

## Tính năng

- **Dịch trực tiếp** âm thanh hệ thống, micro, hoặc cả hai cùng lúc.
- **Nhiều engine:** Soniox, OpenAI Realtime, Qwen; trên Mac chip Apple có thêm engine chạy hoàn toàn
  offline (MLX).
- **Dịch hai chiều** cho cuộc trò chuyện giữa hai ngôn ngữ.
- **Đọc to bản dịch** bằng nhiều giọng đọc, kể cả giọng offline.
- **Dịch nhanh đoạn chữ đang bôi đen** trong bất kỳ app nào.
- **Ghim cửa sổ** nổi trên mọi app, kể cả khi app khác đang toàn màn hình.
- **Lưu lịch sử** từng phiên, tìm kiếm, xuất ra `.srt` (phụ đề) hoặc `.txt`.

## Cài đặt

**macOS** — mở file `.dmg`, kéo Glossa vào Applications. Lần đầu dùng, macOS sẽ hỏi quyền:

- *Screen & System Audio Recording* — để nghe âm thanh hệ thống. Bật xong cần mở lại app.
- *Microphone* — khi dịch từ micro.
- *Accessibility* — chỉ khi dùng tính năng dịch chữ đang bôi đen.

Nếu macOS báo không mở được app, bấm chuột phải vào Glossa trong Applications → **Open** → **Open**.

**Windows** — chạy file `-setup.exe`. Nếu Windows SmartScreen hiện cảnh báo, bấm **More info** →
**Run anyway**. Khi dịch từ micro, bật *Settings → Privacy & security → Microphone* cho app desktop.

## Bắt đầu

1. Mở **Cài đặt**, chọn engine và dán API key của engine đó (Soniox, OpenAI hoặc Qwen). Engine
   offline trên Mac không cần key.
2. Chọn ngôn ngữ nguồn và ngôn ngữ đích.
3. Chọn nguồn âm thanh (hệ thống / micro / cả hai) và bấm bắt đầu.

## Quyền riêng tư

Glossa không có máy chủ riêng. Âm thanh được gửi thẳng từ máy bạn tới engine bạn chọn, bằng API key
của chính bạn; với engine offline thì không rời khỏi máy. Bản ghi và cài đặt chỉ lưu trên máy bạn.

## Gặp lỗi?

Trên Windows, nếu app đang nghe mà không ra chữ, hãy gửi kèm file `%TEMP%\glossa_audio.log` khi báo
lỗi — file này cho biết app đã mở thiết bị âm thanh nào và có nghe thấy gì không.

---

<a id="english"></a>

# Glossa

[Tiếng Việt](#glossa) · **English**

Live speech translation on your desktop: Glossa listens to your system audio or microphone and shows
the translation while the speaker is still talking — for meetings, videos, livestreams and lectures.

This repo holds Glossa's releases only, and is where the app checks for updates.

## Download

Go to the [latest release](https://github.com/CongThang1597/glossa-releases/releases/latest) and pick:

| System | File |
|---|---|
| macOS 13 or later, Apple silicon (M1 or later) | `Glossa_<version>_aarch64.dmg` |
| Windows 10 / 11 (64-bit) | `Glossa_<version>_x64-setup.exe` (or `.msi`) |

After the first install, Glossa tells you when a new version is out — click **Cập nhật** (Update)
and it installs itself.

## Features

- **Live translation** of system audio, the microphone, or both at once.
- **Several engines:** Soniox, OpenAI Realtime, Qwen; on Apple-silicon Macs, a fully offline engine
  (MLX) as well.
- **Two-way mode** for a conversation between two languages.
- **Reads translations aloud** with a choice of voices, offline ones included.
- **Translates highlighted text** in any app.
- **Pins its window** above every app, even one in full screen.
- **Keeps a history** of every session — searchable, exportable as `.srt` subtitles or `.txt`.

The app's interface is in Vietnamese.

## Install

**macOS** — open the `.dmg` and drag Glossa into Applications. On first use macOS asks for:

- *Screen & System Audio Recording* — to hear system audio. Reopen the app after turning it on.
- *Microphone* — when translating from the microphone.
- *Accessibility* — only for translating highlighted text.

If macOS says the app cannot be opened, right-click Glossa in Applications → **Open** → **Open**.

**Windows** — run the `-setup.exe`. If Windows SmartScreen warns you, click **More info** →
**Run anyway**. To translate from the microphone, allow desktop apps under
*Settings → Privacy & security → Microphone*.

## Getting started

1. Open **Cài đặt** (Settings), choose an engine and paste its API key (Soniox, OpenAI or Qwen). The
   offline engine on Mac needs no key.
2. Choose the source and target languages.
3. Choose the audio source (system / microphone / both) and start.

## Privacy

Glossa has no server of its own. Audio goes straight from your computer to the engine you picked,
with your own API key; with the offline engine it never leaves your machine. Transcripts and
settings are stored on your computer only.

## Something wrong?

On Windows, if the app is listening but no text appears, attach `%TEMP%\glossa_audio.log` to your
report — it shows which audio device the app opened and whether it heard anything.
