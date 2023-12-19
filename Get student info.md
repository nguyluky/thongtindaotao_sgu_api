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
 ```ts
 type infoResponse = {
  data: {
    thoi_gian_get_data: "DD/MM/YYYY hh:mm:ss",
    ma_sv: string,
    ten_day_du: string,
    gioi_tinh: "Nam" | "Nữ",
    ngay_sinh: "DD/MM/YYYY",
    noi_sinh: string,
    dan_toc: string,
    ton_giao: string,
    quoc_tich: string,
    dien_thoai: string,
    email: string,
    dien_thoai2: string,
    email2: string,
    doi_mat_khau: false | true,
    so_cmnd: string,
    ho_khau_thuong_tru_gd: string,
    lop: string,
    khu_vuc: string,
    doi_tuong_uu_tien: string,
    doi_tuong_xet_TN: string,
    khoi: string,
    nganh: string,
    chuyen_nganh: string,
    id_chuyen_nganh: string,
    khoa: string,
    bac_he_dao_tao: string,
    nien_khoa: "from_YYYY-to_YYYY",
    ma_cvht: string,
    ho_ten_cvht: string,
    email_cvht: string,
    dien_thoai_cvht: string,
    ma_cvht_ng2: "",
    ho_ten_cvht_ng2: "",
    email_cvht_ng2: "",
    dien_thoai_cvht_ng2: "",
    ma_truong: string,
    ten_truong: string,
    id_dia_phuong: string,
    id_khoa: string,
    id_sinh_vien: string,
    id_lop: string,
    id_khoi: string,
    id_bac_he_nganh: string,
    id_bac_he: string,
    id_he: string,
    id_quy_che: string,
    id_quy_che_P: string,
    id_hoc_che: string,
    id_don_vi_phan_cap: string,
    id_co_so_lop: "0",
    nhhk_vao: number,
    nhhk_ra: number,
    id_lop2: "0",
    id_khoi2: "0",
    id_bac_he_nganh2: "0",
    is_master_pass: boolean,
    is_cvht_dang_nhap: boolean,
    is_phu_huynh_dang_nhap: boolean,
    number_hien_dien_sv: 0,
    hien_dien_sv: string,
    number_hien_dien_dkmh: 0,
    ds_menu_cam_xem: [],
    str_hoan_thanh_dgrl: "",
    url_netweb: ""
  },
  "result": boolean,
  "code": number
}
 ```