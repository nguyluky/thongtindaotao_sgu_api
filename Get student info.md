# Get student Info
Get student info (ex. industry code, class)

Method: `POST`  
URL: `https://thongtindaotao.sgu.edu.vn/api/dkmh/w-locsinhvieninfo`  
Headers:  
 - `Content-Type`: `application/json`  
 - `Authorization`: `Bearer {access_token}`

Variables:  
 - `{access_token}` : Read [auth](auth.md)


Response:  
 ```json
 {
  "data": {
    "thoi_gian_get_data": "DD/MM/YYYY hh:mm:ss",
    "ma_sv": String,
    "ten_day_du": String,
    "gioi_tinh": "Nam" | "Nữ",
    "ngay_sinh": "DD/MM/YYYY",
    "noi_sinh": String,
    "dan_toc": String,
    "ton_giao": String,
    "quoc_tich": String,
    "dien_thoai": String,
    "email": String,
    "dien_thoai2": String,
    "email2": String,
    "doi_mat_khau": false | true,
    "so_cmnd": String,
    "ho_khau_thuong_tru_gd": String,
    "lop": String,
    "khu_vuc": String,
    "doi_tuong_uu_tien": Sting,
    "doi_tuong_xet_TN": String,
    "khoi": String,
    "nganh": String,
    "chuyen_nganh": String,
    "id_chuyen_nganh": String,
    "khoa": String,
    "bac_he_dao_tao": String,
    "nien_khoa": "from_YYYY-to_YYYY",
    "ma_cvht": String,
    "ho_ten_cvht": String,
    "email_cvht": String,
    "dien_thoai_cvht": String,
    "ma_cvht_ng2": "",
    "ho_ten_cvht_ng2": "",
    "email_cvht_ng2": "",
    "dien_thoai_cvht_ng2": "",
    "ma_truong": String,
    "ten_truong": String,
    "id_dia_phuong": String,
    "id_khoa": String,
    "id_sinh_vien": String,
    "id_lop": String,
    "id_khoi": String,
    "id_bac_he_nganh": String,
    "id_bac_he": String,
    "id_he": String,
    "id_quy_che": String,
    "id_quy_che_P": String,
    "id_hoc_che": String,
    "id_don_vi_phan_cap": String,
    "id_co_so_lop": "0",
    "nhhk_vao": Int,
    "nhhk_ra": Int,
    "id_lop2": "0",
    "id_khoi2": "0",
    "id_bac_he_nganh2": "0",
    "is_master_pass": Bool,
    "is_cvht_dang_nhap": Bool,
    "is_phu_huynh_dang_nhap": Bool,
    "int_hien_dien_sv": 0,
    "hien_dien_sv": String,
    "int_hien_dien_dkmh": 0,
    "ds_menu_cam_xem": [],
    "str_hoan_thanh_dgrl": "",
    "url_netweb": ""
  },
  "result": Bool,
  "code": Int
}
 ```