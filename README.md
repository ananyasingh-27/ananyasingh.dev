# Ananya Singh — portfolio

Source for Ananya's personal website. The site is buildless HTML, CSS, and JavaScript; the files in this repository root are the files to publish at `ananyasingh.dev`.

## Local preview

From this directory, run `python3 -m http.server 8000` and open `http://localhost:8000`.

## Résumé

`resume.yaml` is the editable RenderCV source for the **public** résumé. It intentionally omits a phone number. To rebuild it, install the pinned dependencies in `requirements.txt`, then run:

```sh
rendercv render resume.yaml --output-folder generated
cp generated/Ananya_Singh_CV.pdf ananya-singh-resume.pdf
```

Review the generated PDF and its metadata before publishing. Keep private application-specific résumé versions and any credentials out of this repository.

## Deployment

Cloudflare Pages can deploy this static repository with no build command and the repository root (`/`) as the output directory. The custom domain is `ananyasingh.dev`.
