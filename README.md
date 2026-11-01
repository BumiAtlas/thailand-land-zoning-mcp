# Thailand Land Parcels, Public Land & Zoning MCP (ที่ดินและผังเมืองรวม)

[ภาษาไทย](#ภาษาไทย)

Connect your AI assistant to [BumiAtlas](https://bumiatlas.com) for Thai land research through the Model Context Protocol.

This listing is a focused entry point for:

- Land parcels from the Department of Lands' (DOL) public LandsMaps layer: boundary, survey sheet number and area from the outline
- Public land with an NSL certificate (นสล., ~123k plots nationwide): certificate id, holder and use, area, village, tambon, amphoe, province and land office
- Comprehensive-plan (ผังเมืองรวม) zoning at any point: DPT province and town plans and Bangkok's city plan, with land use and, where set, FAR, building coverage, open space ratio, height and minimum lot size
- The zoning over a parcel, with each zone's share of it

Parcels are loaded for some areas so far; public land and zoning cover the whole country where plans are published. The public parcel layer has no deed (chanote) number, owner or price.

## Connect

```
https://bumiatlas.com/mcp/thailand
```

Add it as a custom connector in any MCP client and sign in with Google. Tools, examples and data notes: [bumiatlas.com/mcp-docs/thailand](https://bumiatlas.com/mcp-docs/thailand).

## Tools

| Tool | Description |
|---|---|
| `TH_parcel_search` | Parcels and public land at `latitude, longitude`, or public land by NSL id (e.g. UB5004) |
| `TH_parcel_get` | One parcel: survey sheet number, area and the plan zones covering it; boundary as GeoJSON |
| `TH_parcel_image` | Satellite or street map image of a parcel or point, with every parcel in view outlined and labelled with its land number |
| `TH_public_land_get` | One NSL public land plot: holder and use, area, place, land office and zoning; boundary as GeoJSON |
| `TH_zoning_get` | Comprehensive-plan zones at a point or by id: land use, plan, and FAR, coverage and height limits where set |

## Example prompts

- *"What is the zoning at 13.7563, 100.5018 in Bangkok? What floor area ratio is allowed?"*
- *"Which parcel is at 13.8231, 100.5100, and how big is it?"*
- *"Is there public land near this point in Nonthaburi? Who holds it?"*
- *"Look up NSL certificate UB5004."*

## Data sources

Parcels and public land © กรมที่ดิน (Department of Lands, DOL), LandsMaps. Zoning © กรมโยธาธิการและผังเมือง (Department of Public Works and Town & Country Planning, DPT); Bangkok's city plan © Bangkok Metropolitan Administration.

## ภาษาไทย

เชื่อมต่อผู้ช่วย AI ของคุณกับ [BumiAtlas](https://bumiatlas.com) เพื่อค้นหาข้อมูลที่ดินในประเทศไทยผ่าน Model Context Protocol (MCP)

- แปลงที่ดินจากชั้นข้อมูลสาธารณะ LandsMaps ของกรมที่ดิน: รูปแปลง เลขที่ดิน และเนื้อที่ที่คำนวณจากรูปแปลง
- ที่ดินของรัฐที่มีหนังสือสำคัญสำหรับที่หลวง (นสล.) ทั่วประเทศ: เลขที่ นสล. หน่วยงานที่ดูแลและการใช้ประโยชน์ เนื้อที่ ที่ตั้ง และสำนักงานที่ดินที่รับผิดชอบ
- ผังเมืองรวมของกรมโยธาธิการและผังเมือง (ผังเมืองรวมจังหวัดและผังเมืองรวมเมือง/ชุมชน) และผังเมืองรวมกรุงเทพมหานคร: ประเภทการใช้ประโยชน์ที่ดิน และ FAR, BCR, OSR, ความสูง และขนาดแปลงขั้นต่ำ เมื่อผังกำหนดไว้

ข้อมูลแปลงที่ดินสาธารณะไม่มีเลขโฉนด ชื่อเจ้าของ หรือราคา และขณะนี้มีข้อมูลแปลงที่ดินเพียงบางพื้นที่

**เชื่อมต่อ:** เพิ่ม `https://bumiatlas.com/mcp/thailand` เป็น custom connector ในโปรแกรมที่รองรับ MCP แล้วลงชื่อเข้าใช้ด้วย Google ผู้ช่วยจะตอบเป็นภาษาไทยได้ แม้ชื่อเครื่องมือจะเป็นภาษาอังกฤษ

ตัวอย่างคำถาม:

- *"ที่พิกัด 13.7563, 100.5018 ในกรุงเทพฯ อยู่ในผังเมืองประเภทไหน และ FAR เท่าไร"*
- *"แปลงที่ดินที่พิกัด 13.8231, 100.5100 คือแปลงไหน เนื้อที่เท่าไร"*
- *"มีที่ดินของรัฐใกล้จุดนี้ในนนทบุรีไหม หน่วยงานไหนดูแล"*
- *"ค้นหา นสล. เลขที่ UB5004"*
