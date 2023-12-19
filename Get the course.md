# get the course

get list class, course, industry code

Method: `POST`  
URL: `https://thongtindaotao.sgu.edu.vn/api/dkmh/w-locdsnhomto`  
Headers:  
 - `Content-Type`: `application/json`  
 - `Authorization`: `Bearer {access_token}`

Variables:  
 - `{access_token}` : Read [auth](auth.md)


Body: 
 ```json
 {
  "is_CVHT": false,
  "additional": {
    "paging": {
      "limit": 8000,
      "page": 1
    },
    "ordering": [
      {
        "name": "",
        "order_type": ""
      }
    ]
  }
}
 ```

Response:
 ```json
 {
  "data": {
    "total_items": Int,
    "total_pages": Int,
    "dien_giai_enable_chung": String,
    "ghi_chu_dkmh": String,
    "trong_thoi_gian_dang_ky": Bool,
    "trong_thoi_gian_duyet_kqdk": Bool,
    "hien_cot_tach_phieu_nop_tien": Bool,
    "addin_duyet_kqdk": Bool,
    "hien_cot_hoc_phi": Bool,
    "hien_cot_ma_lop": Bool,
    "hien_thi_cot_lich_thi": Bool,
    "hoc_ky_dang_ky": String,
    "is_show_tietbd": Bool,
    "is_merge_dong_tkbhk": Bool,
    "ds_khoa": [
      {
        "ma": String,
        "ten": String
      },
      ...
    ],
    "ds_lop": [
      {
        "ma": String,
        "ten": String
      },
      ...
    ],
    "ds_nhom_to": [
      {
        "id_to_hoc": String,
        "id_mon": String,
        "ma_mon": String,
        "ten_mon": "",
        "so_tc": String,
        "so_tc_so": Int,
        "is_vuot": Bool,
        "nhom_to": String,
        "to": "",
        "lop": String,
        "ds_lop": [
          String,
          ...
        ],
        "ds_khoa": [
          String,
          ...
        ],
        "is_kdk": Bool,
        "sl_dk": Int, // đã đăng ký
        "sl_cp": Int, // tổng cộng
        "sl_cl": Int, // còn lại slot
        "tkb": String,
        "is_hl": Bool,
        "enable": Bool,
        "hauk": Bool,
        "is_dk": Bool,
        "gc_enable": String,
        "is_rot": Bool,
        "is_ctdt": Bool,
        "is_chctdt": Bool,
        "is_kg_lt": Bool,
        "thu": 0,
        "tbd": 0,
        "so_tiet": 0,
        "is_kg_huy_kqdk": Bool
      },
      ...
    ]
  },
  "result": Bool,
  "code": Int,
  "time": ""
}
 ```
