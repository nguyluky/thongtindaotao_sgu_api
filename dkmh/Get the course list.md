# get the course

get list class, course, industry code

Method: `POST`  
URL: `https://thongtindaotao.sgu.edu.vn/public/api/dkmh/w-locdsnhomto`  
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
 ```ts
type CourseListResponse = {
  data: {
    total_items: number,
    total_pages: number,
    dien_giai_enable_chung: string,
    ghi_chu_dkmh: string,
    trong_thoi_gian_dang_ky: boolean,
    trong_thoi_gian_duyet_kqdk: boolean,
    hien_cot_tach_phieu_nop_tien: boolean,
    addin_duyet_kqdk: boolean,
    hien_cot_hoc_phi: boolean,
    hien_cot_ma_lop: boolean,
    hien_thi_cot_lich_thi: boolean,
    hoc_ky_dang_ky: string,
    is_show_tietbd: boolean,
    is_merge_dong_tkbhk: boolean,
    ds_khoa: {
      ma: string,
      ten: string
    }[],
    ds_lop: {
      ma: string,
      ten: string
    }[],
    ds_nhom_to:{
        id_to_hoc: string,
        id_mon: string,
        ma_mon: string,
        ten_mon: "",
        so_tc: string,
        so_tc_so: number,
        is_vuot: boolean,
        nhom_to: string,
        to: "",
        lop: string,
        ds_lop: string[],
        ds_khoa: string[],
        is_kdk: boolean,
        sl_dk: number, // đã đăng ký
        sl_cp: number, // tổng cộng
        sl_cl: number, // còn lại slot
        tkb: string,
        is_hl: boolean,
        enable: boolean,
        hauk: boolean,
        is_dk: boolean,
        gc_enable: string,
        is_rot: boolean,
        is_ctdt: boolean,
        is_chctdt: boolean,
        is_kg_lt: boolean,
        thu: 0,
        tbd: 0,
        so_tiet: 0,
        is_kg_huy_kqdk: boolean
      }[],
  },
  result: boolean,
  code: number,
  time: ""
}
 ```
