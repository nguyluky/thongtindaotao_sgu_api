# Get Registered Course

Method: `POST`  
URL: `https://thongtindaotao.sgu.edu.vn/api/dkmh/w-locdskqdkmhsinhvien`  
Headers:  
 - `Content-Type`: `application/json`  
 - `Authorization`: `Bearer {access_token}`

Variables:  
 - `{access_token}` : Read [auth](auth.md)

Body:  
 ```json
 {
    "is_CVHT": false,
    "is_Clear": false
 }
 ```

Response:  
 ```json
 {
  "data": {
    "total_items": Int,
    "total_pages": Int,
    "so_tin_chi_min": Int,
    "ngay_in": "YYYY-MM-DDThh:mm:ss+07:00",
    "is_show_nganh_hoc": Bool,
    "ds_kqdkmh": [
      {
        "id_kqdk": String,
        "trang_thai_mon": String,
        "ngay_dang_ky": String,
        "nguoi_dang_ky": "{username}_web",
        "is_da_rut_mon_hoc": Bool,
        "enable_xoa": Bool,
        "dien_giai_enable_xoa": String,
        "hoc_phi_tam_tinh": 0,
        "to_hoc": {
          "id_to_hoc": String,
          "id_mon": String,
          "ma_mon": String,
          "ten_mon": String,
          "so_tc": String,
          "so_tc_so": Int,
          "is_vuot": Bool,
          "nhom_to": String,
          "lop": String,
          "is_kdk": Bool,
          "sl_dk": 0,
          "sl_cp": 0,
          "sl_cl": 0,
          "tkb": String,
          "is_hl": Bool,
          "enable": Bool,
          "hauk": Bool,
          "is_dk": Bool,
          "is_rot": Bool,
          "is_ctdt": Bool,
          "is_chctdt": Bool,
          "is_kg_lt": Bool,
          "thu": 0,
          "tbd": 0,
          "so_tiet": 0,
          "is_kg_huy_kqdk": Bool
        }
      },
      ...
    ]
  },
  "result": true,
  "code": 200
}
 ```